@startuml
scale 2

abstract class MediosTransporte{
    
}

class TransporteAcuatico{
    -numeroCascos: int
    +navegar(): void
    +avanzar(): void
}

class Barco{
    -tipoBarco: String
    +atracar(): void
}

class Trajinera{
    -tamaño: Int
    +turistear(): void
}

class TransporteAereo{
    -numeroAlerones: int
    +volar(): void
    +avanzar(): void
}

class Avión{
    -capacidad: int
    +salirTiempo(): void
}

class Helicoptero{
    -numeroElices: int
    +descender(): void
}

class TransporteTerrestre{
    -energiaUtilizada: String
    +rodar(): void
    +avanzar(): void
}

class Supraterraneo{
    -numeroLlantas: int
    +derrapar(): void
}

class Subterraneo{
    -numeroBagones: int
    +atrasar(): void
}

class Combi{
    -ruta: int
    +hacerparadas(): void
}
 
class Taxi{
    -numeroTaximetro: int
    +llamar(): void
}

class Metro{
    -largo: int
    +prenderventilador(): void
}

class Suburbano{
    -costo: int
    +precionarPuerta(): void
}

MediosTransporte <|-- TransporteAcuatico 
MediosTransporte <|-- TransporteAereo
MediosTransporte <|-- TransporteTerrestre
TransporteAcuatico <|-- Barco
TransporteAcuatico <|-- Trajinera
TransporteAereo <|-- Avión
TransporteAereo <|-- Helicoptero
TransporteTerrestre <|-- Supraterraneo
TransporteTerrestre <|-- Subterraneo
Supraterraneo <|-- Taxi
Supraterraneo <|-- Combi
Subterraneo <|-- Metro
Subterraneo <|-- Suburbano
@enduml
