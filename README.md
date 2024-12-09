# 🍕 Pizzeria-API

**Pizzeria-API** es una API REST completa desarrollada en Java que permite gestionar de forma eficiente los datos y operaciones de 
una pizzería. Esta aplicación ofrece una estructura robusta para manejar clientes, pedidos y productos (pizzas), además de contar 
con auditorías automáticas mediante JPA.

## 🚀 Características

- **Gestión de clientes:** CRUD completo para los datos de los clientes.
- **Gestión de pedidos:** Manejo de órdenes de compra, con la posibilidad de actualizarlas, eliminarlas y consultarlas.
- **Gestión de pizzas:** CRUD para la información de productos (pizzas).
- **Auditorías JPA:** Registra automáticamente las fechas de creación y modificación de cada entidad en la base de datos.
- **Conexión con MySQL:** Persistencia de datos utilizando Spring Data JPA.
- **Frameworks modernos:** Basado en Java 17, Gradle y Spring Framework 3.0.4.

---

## 🛠️ Tecnologías utilizadas

- **Lenguaje:** Java 17
- **Framework principal:** Spring Framework 3.0.4
- **Dependencias clave:**
  - Spring Web
  - Spring Data JPA
- **Base de datos:** MySQL
- **Manejo de dependencias:** Gradle

---

## 📂 Estructura del proyecto

La estructura del proyecto está organizada de la siguiente manera:
```
src 
└── main 
    ├── java 
    │   └── com.dvchinx.pizza 
    │       ├── persistence 
    │       │   ├── audit    # Clases para auditorías JPA 
    │       │   ├── entity   # Entidades principales 
    │       │   ├── projection  # Proyecciones personalizadas 
    │       │   └── repository  # Repositorios JPA 
    │       ├── service 
    │       │   ├── dto   # Objetos de transferencia de datos 
    │       │   ├── exception   # Manejo de excepciones 
    │       │   ├── CustomerService.java # Lógica de negocio para clientes 
    │       │   ├── OrderService.java    # Lógica de negocio para pedidos 
    │       │   └── PizzaService.java     # Lógica de negocio para pizzas 
    │       └── web.controller 
    │       │   ├── CustomerController.java   # Endpoints REST para clientes 
    │       │   ├── OrderController.java      # Endpoints REST para pedidos 
    │       │   └── PizzaController.java      # Endpoints REST para pizzas 
    │       └── PizzeriaApplication.java      # Clase principal de la aplicación 
    ├── resources 
    │    └── application.properties     # Configuración de la aplicación 
    └── test 
        └── ... # Clases para pruebas
