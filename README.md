1. Apartado sobre la API en el README.md
Cómo se llama: football-data.org


En qué categoría de la lista la encontraste: En la categoría de Sports (Deportes / Fútbol).


Quién la mantiene: Desarrollada y mantenida por Daniel Freitag.


Dónde está su documentación: Documentación oficial de football-data.org


Qué condiciones de uso tiene: Ofrece un plan gratuito (Free Tier) con un límite de peticiones por minuto (habitualmente 10 solicitudes por minuto) que requiere el uso de un token de autenticación (X-Auth-Token), además de opciones de suscripción de pago para mayor volumen y frecuencia de datos.


Qué peticiones has hecho: Peticiones HTTP GET para consultar información sobre competiciones, calendarios de partidos, clasificaciones de ligas (standings) y detalles de los equipos.


2. Tabla de campos de un elemento de la colección (Ejemplo: Objeto Partido / Match)
Tomando como referencia la respuesta en formato JSON de un partido de fútbol dentro de la API, la tabla que relaciona los campos del JSON con su significado visual en la web es la siguiente:
Campo del JSON
Tipo de dato
Qué es para el lector
id
número
El identificador único del partido, que sirve para referenciar el encuentro de forma unívoca.
utcDate
texto (fecha)
La fecha y la hora oficial en formato UTC en la que está programado o se disputa el partido.
status
texto
El estado actual del encuentro (por ejemplo: SCHEDULED, TIMED, IN_PLAY, FINISHED), indicando si ya se jugó, se está jugando o está pendiente.
homeTeam.name
texto
El nombre oficial del equipo que actúa como local, situado a la izquierda en el marcador del partido.
awayTeam.name
texto
El nombre oficial del equipo visitante, situado a la derecha en el marcador del partido.
score.fullTime.home y score.fullTime.away
números
Los goles anotados por el equipo local y visitante al final del tiempo reglamentario, formando el resultado final visible en la tarjeta del partido.


