# Practica_uml
Diagrama empleados
Practica 1 de UML
===
<!--Victor Balladares-->
<!--1º DAM-->

``` mermaid
classDiagram
      
      Empresa <|-- Empleado
      Persona <|-- Empleado
      Directivo <|-- Empleado
      Empresa <|-- Cliente
      Empleado <|-- Directivo : subordinado

    class Persona{
        -Nombre : String
        -Edad : Integer
        -Mostrar() void
    }

    class Empleado{
        -SueldoBruto : Integer
        -Calcular_salario_neto : Integer
        -Mostrar() void
    }


    class Cliente{
        -Telefono de contacto: Integer
        -Mostrar() void
    }

    class Empresa{
        -Nombre : String
        -Cif : String
    }

    class Directivo{
        -Categoria : String
        -Mostrar() void
    }


