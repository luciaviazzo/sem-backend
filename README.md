# Sistema de Estacionamiento Medido (SEM)

Proyecto universitario desarrollado en equipo en el marco de la materia **Programación con Objetos II** de la Universidad Nacional de Quilmes.

## Descripción

Sistema backend para la gestión y control de estacionamientos en una localidad. Permite a los usuarios iniciar y finalizar estacionamientos a través de una app, gestionar su saldo, recibir notificaciones y detectar automáticamente el movimiento del vehículo. Los inspectores pueden verificar infracciones en zonas asignadas.

## Funcionalidades principales

- Inicio y fin de estacionamiento (modo manual y automático)
- Gestión de saldo y recarga de crédito
- Detección de movimiento mediante sensores (estados: Apagado, Caminando, Manejando)
- Generación de infracciones por parte de inspectores
- Notificaciones al usuario ante eventos del sistema
- Validación de estacionamiento vigente por patente
- Manejo de excepciones personalizadas 

## Patrones de diseño aplicados

- **Observer**: el SEM actúa como sujeto y notifica a los suscriptores ante eventos como compras, inicio/fin de estacionamiento, recargas e infracciones.
- **Strategy**: el modo de operación del usuario (Manual / Automático) es intercambiable en tiempo de ejecución.
- **State**: el estado de detección de movimiento del usuario transiciona entre Apagado, Caminando y Manejando.

## Tecnologías

- Java
- JUnit
- Mockito
