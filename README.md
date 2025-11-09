# 🧠 TaskControl

**TaskControl** es una aplicación empresarial inteligente desarrollada con **Flutter (Frontend)** y **C# (.NET Backend)** que permite **organizar, asignar y monitorear tareas operativas** dentro de una empresa de forma eficiente y automatizada.  

Combina inteligencia artificial, algoritmos de distribución de carga y comunicación en tiempo real para optimizar la gestión del trabajo en equipos de cualquier tamaño.

---

## 🚀 Visión del Proyecto

> "Asignar la tarea correcta, a la persona correcta, en el momento correcto."

TaskControl busca transformar la coordinación empresarial a través de:
- Automatización de la asignación de tareas.
- Monitoreo del rendimiento operativo en tiempo real.
- Comunicación interna integrada (chat por tareas y 1:1).
- Análisis de productividad y reportes.

---

## 🏗️ Arquitectura General

| Capa | Tecnología | Descripción |
|------|-------------|-------------|
| **Frontend** | Flutter | Aplicación móvil multiplataforma con interfaz moderna y fluida. |
| **Backend API** | ASP.NET Core (C#) | Gestión de autenticación, asignación de tareas, lógica empresarial y control de usuarios. |
| **Base de Datos** | Azure SQL Database | Almacenamiento de tareas, usuarios, colas, evidencias y reportes. |
| **Comunicación en Tiempo Real** | WebSockets / SignalR | Canal de comunicación bidireccional para chat interno y actualizaciones instantáneas. |
| **Despliegue Cloud** | Azure App Service | Backend y base de datos en la nube con alta disponibilidad. |

---

## ⚙️ Características Principales

### 👥 Gestión de Roles
- **Administrador:** Configura la empresa, sucursales, catálogos y políticas (SLA, turnos, permisos, privacidad).
- **Supervisor:** Crea tareas, controla el flujo de asignaciones, valida cierres y supervisa métricas.
- **Trabajador:** Recibe, acepta o declina tareas; ejecuta y reporta con evidencias.

### 🤖 Asignación Inteligente
- Algoritmo de reparto basado en **habilidades, certificaciones y disponibilidad en tiempo real**.
- Distribución automática y balanceada de carga entre trabajadores.
- Opción de asignación manual en casos especiales.

### 💬 Comunicación Interna
- Chat integrado por tarea y entre usuarios (1:1).
- Actualización en tiempo real mediante **WebSockets**.
- Notificaciones instantáneas (push).

### 📈 Analítica y Monitoreo
- Panel de control con métricas en vivo (tareas activas, tiempos promedio, productividad).
- Reportes personalizados por equipo o empleado.
- Exportación de datos a Excel y Power BI.

### 🔐 Seguridad y Privacidad
- Autenticación JWT con roles y permisos.
- Conexiones seguras (HTTPS / SSL).
- Control de visibilidad de datos según jerarquía.

## 🧮 Algoritmo de Repartición de Tareas (Resumen)

El motor de asignación calcula la **“eficiencia ponderada”** de cada trabajador con base en:
1. Disponibilidad actual (`freeSlots`).
2. Habilidades coincidentes (`skillMatch`).
3. Historial de cumplimiento (`performanceScore`).
4. Distancia o prioridad contextual (`taskWeight`).

Efficiency = (skillMatch * 0.4) + (performanceScore * 0.3) + (1 - queueLoad) * 0.3;
El sistema elige automáticamente al trabajador con mayor eficiencia para cada nueva tarea disponible.
☁️ Infraestructura en Azure

Azure SQL Database: Persistencia relacional.

Azure App Service: Hospedaje del backend .NET.

Azure Blob Storage: Almacenamiento de evidencias (imágenes, documentos).

Azure Notification Hub: Envío de notificaciones push.

SignalR Service: WebSockets administrados para comunicación en tiempo real.

### 🔄 Roadmap

 API base de usuarios y autenticación JWT.

 Módulo de creación y asignación de tareas.

 Integración con Azure SQL.

 Implementación completa de WebSockets (SignalR).

 Dashboard avanzado de métricas.

 Integración de IA para predicción de carga laboral.

 Modo offline para la app móvil.

### 💼 Autor y Equipo

Proyecto académico y empresarial desarrollado por el equipo de TaskControl, con visión de escalar hacia un SaaS de gestión operativa inteligente.

Frontend: Flutter

Backend: ASP.NET Core (C#)

Database: Azure SQL

Realtime: SignalR

Infraestructura: Azure Cloud

### 🧾 Licencia

Este proyecto se distribuye bajo licencia MIT License.
Puedes usarlo, modificarlo y desplegarlo libremente con atribución al autor original.

© 2025 TaskControl — Intelligent Task Management for Enterprises
