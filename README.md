# Ejecución Local

Para iniciar la aplicación localmente se deben ejecutar sus mòdulos por separado:

1.  **Eureka server:**
    Navega al directorio `eureka-server` y ejecuta ```mvn spring-boot:run``. 
    Proporciona el servicio de descubrimiento para los demás módulos, permitiéndoles registrarse y encontrarse entre sí.

2.  **Accreditations:**
    A continuación, ve al directorio `hex-accreditations` y ejecuta ```mvn spring-boot:run``.
    Módulo que gestiona la lógica relacionada con las acreditaciones dentro del sistema.

3.  **Selling points:**
    Luego, dirígete al directorio `hex-selling-point` y ejecuta ```mvn spring-boot:run``. 
    Módulo encargado de implementa las funcionalidades correspondientes a la gestión de puntos de ventas. Creación, edición, borrado y consulta de puntos de venta.

4.  **Api Gateway:**
    Finalmente, accede al directorio `api-getaway` y ejecuta ```mvn spring-boot:run``.
    Actúa como un punto de entrada único para todas las peticiones externas, enrutándolas a los servicios correspondientes.

---

## Ejecución en Entorno Docker

Para desplegar y ejecutar la aplicación utilizando Docker:

1.  **Infraestructura Docker:**
    Desde el directorio `infrastructure`, ejecutar el siguiente comando para construir las imágenes y levantar los contenedores ```docker-compose up --build``.
    Éste módulo contiene el archivo de configuración de Docker Compose para orquestar todos los servicios de la aplicación en contenedores.

---