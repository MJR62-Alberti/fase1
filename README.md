## Apartado sobre la API

* **Cómo se llama:** `football-data.org`
* **Categoría:** Encontrada en la categoría de **Sports (Deportes / Fútbol)**.
* **Mantenimiento:** Desarrollada y mantenida por Daniel Freitag.
* **Documentación oficial:** [Documentación de football-data.org](https://www.football-data.org/documentation)
* **Condiciones de uso:** Ofrece un plan gratuito (*Free Tier*) con un límite de peticiones (habitualmente 10 solicitudes por minuto) que requiere el uso obligatorio de un token de autenticación (`X-Auth-Token`), además de opciones de suscripción de pago para mayor volumen y frecuencia de datos.
* **Peticiones realizadas:** Peticiones HTTP GET para consultar información sobre competiciones, calendarios de partidos, clasificaciones de ligas (*standings*) y detalles de los equipos.

---

## Tabla de campos de un elemento de la colección (Ejemplo: Objeto Partido / *Match*)

Tomando como referencia la respuesta en formato JSON de un partido de fútbol dentro de la API, la tabla que relaciona los campos del JSON con su significado visual en la web es la siguiente:

| Campo del JSON | Tipo de dato | Qué es para el lector |
| :--- | :--- | :--- |
| `id` | Número | El identificador único del partido, que sirve para referenciar el encuentro de forma unívoca. |
| `utcDate` | Texto (fecha) | La fecha y la hora oficial en formato UTC en la que está programado o se disputa el partido. |
| `status` | Texto | El estado actual del encuentro (por ejemplo: `SCHEDULED`, `TIMED`, `IN_PLAY`, `FINISHED`), indicando si ya se jugó, se está jugando o está pendiente. |
| `homeTeam.name` | Texto | El nombre oficial del equipo que actúa como local, situado a la izquierda en el marcador del partido. |
| `awayTeam.name` | Texto | El nombre oficial del equipo visitante, situado a la derecha en el marcador del partido. |
| `score.fullTime.home` / `score.fullTime.away` | Números | Los goles anotados por el equipo local y visitante al final del tiempo reglamentario, formando el resultado final visible en la tarjeta del partido. |
