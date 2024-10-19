# Microservicio de Órdenes

## Descripción
El microservicio de órdenes es esencial para la gestión de pedidos en la aplicación. Este servicio permite a los usuarios crear, consultar y gestionar sus órdenes de manera eficiente. Se integra con otros microservicios, como el de productos y el de pagos, para ofrecer una experiencia de compra completa.

## Funcionalidades
- **Crear Orden**: Permite a los usuarios realizar un pedido de productos, gestionando la información de los productos seleccionados y el estado del pedido.
- **Consultar Órdenes**: Facilita la obtención de detalles de las órdenes, ya sea para un usuario específico o para todos los pedidos en el sistema.
- **Actualizar Estado de la Orden**: Permite actualizar el estado de una orden (por ejemplo, pendiente, completada, cancelada).
- **Eliminar Orden**: Ofrece la opción de cancelar o eliminar órdenes existentes.

## Tecnologías Utilizadas
- **NestJS**: Framework para construir aplicaciones del lado del servidor eficientes y escalables.
- **PostgreSQL**: Sistema de gestión de bases de datos utilizado para almacenar la información de las órdenes.
- **TypeScript**: Lenguaje de programación que proporciona tipado estático, mejorando la calidad del código.
- **Docker**: Facilita la creación y gestión de contenedores para ejecutar el microservicio de manera aislada.
- **NATS**: Sistema de mensajería utilizado para la comunicación asíncrona con otros microservicios, como los de productos y pagos.

## Instalación
Para instalar y ejecutar el microservicio de órdenes, sigue estos pasos:

### 1. Clonar el Repositorio
Clona el repositorio del microservicio:
```bash
git clone https://github.com/TrujiDev/order-microservice.git
cd order-microservice
```

### 2. Instalar Dependencias
Instala las dependencias necesarias utilizando npm:
```bash
npm install
```

### 3. Configuración del Entorno
Crea un archivo `.env` en la raíz del proyecto y configura las variables necesarias:
```env
DATABASE_URL=postgres://user:password@localhost:5432/mydatabase
NATS_URL=nats://localhost:4222
```

### 4. Ejecutar el Microservicio
Finalmente, ejecuta el microservicio:
```bash
npm run start
```

## Uso
El microservicio de órdenes expone las siguientes rutas:

- **POST /orders**: Crea una nueva orden.
- **GET /orders**: Lista todas las órdenes.
- **GET /orders/:id**: Obtiene una orden específica por su ID.
- **PUT /orders/:id**: Actualiza el estado de una orden existente.
- **DELETE /orders/:id**: Elimina una orden del sistema.

## Mantenimiento
Para mantener el microservicio actualizado, asegúrate de:
- Revisar y aplicar actualizaciones de seguridad a las dependencias.
- Realizar pruebas regulares para asegurar el correcto funcionamiento del servicio.

## Contribuciones
Las contribuciones son bienvenidas. Si deseas contribuir a este microservicio, sigue estos pasos:
1. Haz un fork del repositorio.
2. Crea tu feature branch (`git checkout -b feature/AmazingFeature`).
3. Haz un commit de tus cambios (`git commit -m 'Add some AmazingFeature'`).
4. Haz push a la branch (`git push origin feature/AmazingFeature`).
5. Abre un Pull Request.
