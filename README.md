# Las_Dellas-Automatizacion
Desarrollo de una solución integral de e-commerce para un emprendimiento textil, enfocada en la digitalización del ciclo de ventas y la arquitectura de un backend automatizado que elimina la carga administrativa manual en un 100%.

# 🚀 Las Dellas - E-commerce Automation Pipeline

Este proyecto implementa una solución integral de automatización para un emprendimiento textil (**Las Dellas**), transformando un proceso de venta manual en un flujo de datos estructurado y automatizado.

## 📊 Arquitectura del Sistema
El núcleo del proyecto es un orquestador de eventos desarrollado en **n8n** que conecta la captura de datos con la lógica de negocio y la comunicación con el cliente.

![Flujo de Automatización de Las Dellas]<img width="1366" height="605" alt="screenshot-workflow" src="https://github.com/user-attachments/assets/8a9e0678-f984-4fd0-9c96-88b3fee8ebb1" />

## 🛠️ Stack Tecnológico
* **Frontend:** Google Sites (Landing Page).
* **Data Intake:** Google Forms & Google Sheets.
* **Orquestador Backend:** n8n (Self-hosted).
* **Lenguajes:** JavaScript (para transformación de datos dentro del flujo).
* **Notificaciones:** Gmail API.

---

## ⚙️ Funcionamiento Técnico

### 1. Ingesta de Datos (ETL)
El flujo comienza extrayendo filas de un **Google Sheet** que actúa como base de datos centralizada de pedidos. Se asegura la integridad de los datos mediante validaciones en el formulario de entrada.

### 2. Procesamiento y Lógica (JavaScript Node)
Implementé un nodo de **Code en JavaScript** para procesar la información cruda. 
* **Formateo de strings:** Limpieza de nombres y productos.
* **Cálculos lógicos:** Validación de estados de pedido y preparación de variables para el cuerpo del mail.
* **Manejo de JSON:** Estructuración de objetos para la salida hacia los nodos de comunicación.

### 3. Automatización de Salida
* **Envío de Confirmación:** Se dispara un correo automático al cliente con los detalles del pedido procesado.
* **Feedback Loop:** El sistema vuelve a Google Sheets para actualizar el estado del pedido, marcándolo como "Procesado" para evitar duplicados.


## 👤 Autor
**Marcos Griffa** *Estudiante de Ciencia de Datos - Universidad de Buenos Aires (UBA)*
