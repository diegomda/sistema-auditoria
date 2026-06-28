# Sistema de Gestión de Auditorías – Diseño Conceptual

## 📑 Introducción
El sistema busca centralizar la gestión de auditorías internas y externas, optimizando tiempos y asegurando trazabilidad.

## 🎯 Objetivos
- Optimizar tiempos de auditoría.
- Asegurar trazabilidad de incidencias.
- Mejorar comunicación entre áreas.

## 🏗️ Arquitectura
Basada en **PHP + MySQL**, con integración a **Google Drive/OneDrive** para reportes y almacenamiento.

## 🔧 Módulos principales
- **Incidencias**: creación obligatoria con número y proveedor, asignación automática al usuario logueado.
- **Proveedores**: alta y listado desde el navbar.
- **Tablero**: validaciones, modales y botones de navegación.
- **Alertas críticas**: ajustes en notificaciones, eliminación de botón global.

## 📊 Roles y permisos
| Rol                | Puede crear | Puede editar | Puede cerrar | Puede borrar | Comentarios              |
|--------------------|-------------|--------------|--------------|--------------|--------------------------|
| **REGIONAL**       | ❌          | ❌           | ❌           | ❌           | ✅ Puede comentar         |
| **JEFE DE ESTACIÓN** | ✅          | ✅           | ✅           | ✅           | ✅ Puede comentar         |
| **RESPONSABLE DE TURNO** | ✅          | ✅           | ❌ (requiere aprobación JE) | ❌ | ✅ Puede comentar |

## 📈 Diagramas sugeridos
- Organigrama de Roles y Permisos
- Flujo de Incidencias
- Mapa de Navegación del Sistema

## ✅ Validaciones y seguridad
- Formularios con **JavaScript**.
- Control de campos obligatorios.
- Color coding para conflictos.

## 📌 Conclusiones
El sistema asegura transparencia y eficiencia en auditorías, con trazabilidad completa y soporte visual.
