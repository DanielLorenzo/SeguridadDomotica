# Práctica Sistema de Gestión de una empresa de Seguridad

* Todas las interfaces han de implementar el _Diseño para Todos_

## Controlar

* Gestión de los abonados a los servicios ofrecidos
* Revisión de elementos domóticos de las distintas estancias
* Verificación de la seguridad del edificio mediante la detección de alertas de seguridad

## Vertientes de Uso

### Clientes

* Acceso a una interfaz móvil
* Controlar servicios contratados
    * Activar y desactivar
    * Añadir o dar de baja servicios específicos -> Genera modificación en la cuenta mensual
    * Recibir alertas de señal de alarma en la instalación

### Encargado 

* Dispone de información:
    * Sobre abonados
    * Sobre los servicios contratados
    * Central de alarmas

## Manejo

### Cliente

* El cliente controla la domótica

* Ejemplos:
    * Apertura/ciere puertas y ventanas
    * Subir/bajar persianas
    * Encender/apagar luces
    * Controlar sistemas electrónicos

* Los cambios de estados se deben ver reflejados en la interfaz

### Encargado

* Visualizar y controlar las estancias de cada cliente
* Gestión de abonados
    * Controlar las cuotas de abonados
    * Guardar datos personales, servicios contratados y su información importante
        * Dispositivos instalados
        * histórico de señales de alarma
        * Falsas alarmas y relación de reales (robos, atracos, allanamientos, etc.)
        * Listado de claves y personas autorizadas con datos de contacto
        * Comunicaciones a FCS (policía nacional o local, guardia civil, mossos, ertzaintza…)
        * listado de incidencias técnicas del sistema
        * mantenimientos periódicos
        * presencia de animales domésticos en la instalación
    * Gestión de los recursos ofertados
        * alarmas con conexión
        * alarmas sin conexión
        * alarmas de incendio
        * sistemas anti-hurtos
        * sistemas GPS
        * cajas fuertes
        * circuitos cerrados de televisión (CCTV)
        * extintores…
* Central de alarmas
    * Control automático de señales (Aperturas, Cierres, Averías, Temperaturas…)
    * Seguimiento constante de las señales emitidas por los detectores de presencia por estancia
    * Gestión de la temperatura de cada estancia
    * Estado de los ascensores
        * Señales de alarma
        * Mantenimientos necesrarios y periódicos
        * Gestión de casos de avería
            * Parones entre plantas
            * Bloqueo de puertas
            * ...

## Clasificación de estancias

### Despachos

* Control de ventanas y persianas
* puertas
* luces
* temperatura
* sistemas electrónicos:
    * teléfono
    * fax
    * encendido/apagado ordenador

### Salas de trabajo común

Presencia de varios puestos dónde se deberá controlar:

* Elementos del despacho
* Encendido/apagado fotocopiadora
* Cafetera
* Microondas
* Luces individuales de cada puesto

### Baños

* Luces
* Fugas de agua

### Sala de servidores

* Comprobar adecuada refrigeración
* Caídas de servidores
* Cortes de luz
    * Deben provocar que las fuentes auxiliares se activen para que no se apague ningún servidor
* Alarma especial contra intrusos

## Simulación de prototipo

Edificio con:

* Puerta de entrada
* Cinco plantas
* Dos ascensores
* Cuatro despachos
* Una sala de trabajo común
    * 10 puestos individuales
* Cuatro baños
* Sala de servidores