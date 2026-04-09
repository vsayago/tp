# Propuesta TP DSW

## Grupo
### Integrantes
* 53948 – Altamirano, Marianela Estefanía
* 54027 – Sayago, Valentina Nair
* 54207 – Spirce, Yasmín
 
### Repositorios
* Frontend: https://github.com/dsw-2026/frontend
* Backend: https://github.com/dsw-2026/backend

## Tema: Adopción de Mascotas
### Descripción

Sistema de gestión de adopción de mascotas que conecta adoptantes con publicadores (refugios y rescatistas). Permite registrar usuarios, publicar animales disponibles, evaluar la compatibilidad entre adoptantes y mascotas, y dar seguimiento a cada caso de adopción. Su objetivo es agilizar el proceso de adopción y garantizar vínculos responsables y duraderos.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Macota<br>3. CRUD Provincia|
|CRUD dependiente|1. CRUD Solicitud {depende de} CRUD Adoptante, CRUD Mascota<br>2. CRUD Cliente {depende de} CRUD Característica {depende de} CRUD Mascota|
|Listado<br>+<br>detalle| 1. Listado de mascotas disponibles para adoptar filtrado por especie, muestra nombre, imagen, edad, tamaño, sexo, caracter, energia, vacunación y castración => detalle muestra datos completos de la mascota<br> 2. Listado de solicitudes de adopción en proceso, filtrado por fecha descendente, muestra código de adopción, nombre adoptante, nombre publicador, días transcurridos desde fecha solicitud  => detalle CRUD Solicitud|
|CUU/Epic|1. Solicitar adopción de una mascota<br>2. Publicar mascota en adopción|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuario<br>2. CRUD Adoptante<br>3. CRUD Publicador<br>4. CRUD Mascota<br>5. CRUD Solicitud<br>6. CRUD Formulario<br>7. CRUD Historial_seguimiento<br>8. CRUD Característica<br>9. CRUD Especie<br>10. CRUD Raza<br>11. CRUD Provincia<br>12. CRUD Localidad|
|CUU/Epic|1. Solicitar adopción de una mascota<br>2. Publicar mascota nueva en adopción<br>3. Adoptar una mascota|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

