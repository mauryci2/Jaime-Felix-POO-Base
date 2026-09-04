# Proyecto: POO

Platilla base para ejercicios de la materia de POO

## Diagrama de clases
[Editor en línea](https://mermaid.live/)
```mermaid
---
title: Diagrama de Clases
---
classDiagram
      class Biblioteca{
            -List~libro~ inventario
            -List~Lector~ lectores
            +Biblioteca()
            +prestar(Lector lector, Libro libro)
            +devolver(Lector lector, Libro libro)
            
      }
            
      class Libro{
            -id
            -nombre
            -estado
            -estaOcupado
            -tipoLibro
            -editorial
            -autor
            -anio
            -diasPrestados
            +Libro()
            +getDiasPrestados()
            +reiniciarDiasPrestado()
            +getEstado()
            +DetallesLibro()
            +isOcupado()
      }
      class Lector{
            -id
            -cantPrestados
            +Lector()
            +getCantidadPrestados()
            +puedePedir()
            +agregarMulta(int diasRetraso)
            +leer()
            }
      class Ejemplar {
            -String id
            -Libro libro
            -String estado
            +Ejemplar()
            +getEstado()
            +setEstado(String nuevoEstado)
      }
      class Autor{
            -nacionalidad
            -fechaNacimiento
            +Autor()
            +getNacionalidad()
            +getFechaNacimiento()
      }
      class Persona{
            -nombre
            -edad
            +Persona()
            +getNombre()
            +setNombre(String nom)
            +getEdad()
            +setEdad(int edad)
      }
```
[Referencia-Mermaid](https://mermaid.js.org/syntax/classDiagram.html)


## Comandos Git-Cambios y Actualizaciones

### Por cada cambio importante que haga, actualice su historia usando los comandos:
```
git add .
git commit -m "Descripción del cambio"
git push origin main
```
