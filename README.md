# Proyecto: POO

Platilla base para ejercicios de la materia de POO

## Diagrama de clases
[Editor en línea](https://mermaid.live/)
```mermaid
---
title: Aplicación de Computadora
---
classDiagram
      class AppComputadora{
            +static void main(String args[])
      }
      class Empresa{
            -empleado
            -cliente
            +Empresa()
            +getEmpleado()
            +getCliente()
            +contratar(Empleado emp)
            +registrarCliente(Cliente c)
      }
      class Directivo{
            -static categoria;
            -List<Empleado> subordinados
            +Directivo()
            +getCategoria()
            +getSubordinados()
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
      class Empleado{
            -id
            -sueldo
             +Empleado()
            +getId()
            +getSueldo()
            +setSueldo(double sueldo)
      }
      class Cliente{
            -id
            -contacto
            +Cliente()
            +getId()
            +getContacto()
            +setContacto(Contacto c)
            +comprar()
      }
      class Contacto{
            -String numero
            -String correo
            -String contrasenia
            +Contacto()
            +getNumero()
            +setNumero(String num)
            +getCorreo()
            +setCorreo(String c)
            +getContra()
            +setContra(String contra)
            +recibirMensaje(String mensaje)
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
