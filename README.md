# 🚗 Service Order Management System

### Desktop Application for Automotive Service Management

Sistema de gestión de **órdenes de servicio para concesionarias automotrices**, desarrollado como aplicación de escritorio en **C# y .NET**.

El software permite registrar, administrar y generar **órdenes de mantenimiento de vehículos**, facilitando el seguimiento de servicios realizados, la gestión de turnos y la administración de clientes y vehículos.

Este proyecto fue desarrollado tomando como caso real la operatoria del concesionario **Gelardi SRL – Honda Bahía Blanca**.

---

El Service realizado sobre el vehículo se detalla en una ORDEN DE SERVICIO la cual se muestra y es completada a mano alzada.

![orden de servicio](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/d88a341e-6d15-4504-b739-31944c69a7c4)

---

# 📌 Project Overview

En concesionarias automotrices, cada mantenimiento realizado a un vehículo se registra mediante una **Orden de Servicio**.

Este sistema permite digitalizar ese proceso, reemplazando el registro manual por una **aplicación de escritorio que permite:**

* registrar órdenes de servicio
* gestionar clientes
* gestionar vehículos
* gestionar turnos de mantenimiento
* generar órdenes imprimibles
* consultar historial de servicios

El objetivo es mejorar la **organización, trazabilidad y eficiencia administrativa** del proceso de post-venta.

En el siguiente enlace se encuentra el diagrama de la base de datos.
[Diagram_0.pdf](https://github.com/mmontana83/Gelardi-OrdenServicio/files/12134944/Diagram_0.pdf)

A continuación algunas capturas de pantalla
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/a42d1d59-5820-491b-a20b-ba1b116b24f8)

![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/95b2e9b9-c95d-469e-9e6c-2175a53150ae)

![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/309d1c79-e235-4f3b-bcad-8be93add2ed0) ![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/1f817b3a-3fd8-4f1c-acda-4450580c8c7c) ![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/c407e676-76c9-48d0-bbc9-47d67eae9bf6)

Orden de Servicio a Completar.
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/ad7f169f-5bd3-42e3-8aae-303c40d9529b)

Orden de Servicio generada con Crystal Report
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/7f8bd1f9-d25c-407b-aa93-010229e088b5)

Detalle de las órdenes de servicio
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/c047decf-6532-401a-b74d-9c3e1dae6102)

Gestión de Turnos
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/c1fe4e49-72ee-40e8-a237-9f7ceba4f694)
![image](https://github.com/mmontana83/Gelardi-OrdenServicio/assets/101347311/42945f6d-bde1-47e3-bfde-71139e0df422)

---

# ⚙️ Tech Stack

### Language

* C#

### Framework

* .NET (Windows Desktop Application)

### UI Technology

* Windows Forms

### Data Access

* Typed DataSets (.xsd)

### Reporting

* Crystal Reports

### Database

* Relational Database (SQL based)

---

# 🧠 System Architecture

Arquitectura típica de aplicaciones de escritorio empresariales.

```
User Interface
(Windows Forms)
        │
        ▼
Business Logic
(C#)
        │
        ▼
Data Access Layer
(Typed DataSet)
        │
        ▼
Database
(Relational DB)
        │
        ▼
Crystal Reports
(Printable Service Orders)
```

---

# 📊 Main Features

### 🚗 Service Orders

Permite crear y administrar órdenes de servicio asociadas a un vehículo.

Cada orden incluye:

* datos del cliente
* datos del vehículo
* kilometraje
* tipo de mantenimiento
* observaciones técnicas
* fecha de servicio

Las órdenes pueden **guardarse, consultarse e imprimirse**.

---

### 👤 Client Management

Gestión completa de clientes:

* alta de clientes
* modificación de datos
* consulta de clientes
* historial de servicios asociados

---

### 🚘 Vehicle Management

Registro de vehículos asociados a clientes:

* marca
* modelo
* dominio
* kilometraje
* historial de mantenimiento

---

### 📅 Appointment Scheduling

Gestión de turnos para mantenimiento:

* asignación de turnos
* control de disponibilidad
* organización de agenda del taller

---

### 🧾 Service Order Printing

El sistema genera **órdenes de servicio imprimibles** utilizando **Crystal Reports**, permitiendo entregar al cliente un documento formal del servicio realizado.

---

# 🗄 Database Model

El sistema utiliza una base de datos relacional estructurada alrededor de las siguientes entidades principales:

* Clientes
* Vehículos
* Órdenes de Servicio
* Turnos

El acceso a los datos se realiza mediante **Typed DataSets de .NET**.

---

# 📂 Project Structure (Conceptual)

```
Gelardi
│
├── Forms
│   ├── ServiceOrderForm
│   ├── ClientForm
│   ├── VehicleForm
│   └── AppointmentForm
│
├── Data
│   └── GelardiDataSet
│
├── Reports
│   └── CrystalReports
│
└── Business Logic
```

---

# 🖥 User Interface

La aplicación incluye distintas pantallas para la gestión del sistema:

* Registro de clientes
* Registro de vehículos
* Gestión de turnos
* Gestión de órdenes de servicio
* Consulta de historial
* Generación de reportes

---

# 🧪 Running the Project

Requisitos:

* Visual Studio
* .NET Framework
* Crystal Reports Runtime
* Base de datos configurada

Pasos:

1. Clonar el repositorio
2. Abrir la solución en Visual Studio
3. Configurar la conexión a base de datos
4. Ejecutar el proyecto

---

# 💡 Technical Concepts Demonstrated

Este proyecto demuestra experiencia en:

* desarrollo de aplicaciones de escritorio empresariales
* modelado de bases de datos relacionales
* generación de reportes profesionales
* gestión de información transaccional
* diseño de interfaces WinForms
* integración con herramientas de reporting

---

# 🔮 Possible Improvements

* migración a arquitectura **MVC o Clean Architecture**
* reemplazo de DataSets por **Entity Framework**
* API backend para integración con web
* dashboard de métricas
* sistema multiusuario
* almacenamiento en la nube

---

# 👨‍💻 Author

**Martín Montaña**

Analista de Sistemas
Full Stack Developer

Intereses profesionales:

* Software Engineering
* Business Applications
* Backend Development
* Databases
* System Architecture

---

# ⭐ Support

Si el proyecto te resulta interesante, podés darle una ⭐ al repositorio.






