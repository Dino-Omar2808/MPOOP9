@startuml
scale 8

abstract class MediosTransporte{
    
}

class TransporteAcuatico{
    -velocidad: int
    -capacidad: String
    +aumnetarVelocidad(): void
}

class Barco{
    -puertoOrigen: String
    -puertoDestino: String
    +abordarPasajeros(): void
}

MediosTransporte <|-- TransporteAcuatico 
TransporteAcuatico <|-- Barco : interfaz
@enduml


