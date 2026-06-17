# Instalación y Configuración de MySQL

Manual de instalación y configuración del motor de base de datos **MySQL Server** y la herramienta visual **MySQL Workbench**, desarrollado como parte de la actividad práctica de onboarding.

---


| Campo | Detalle |
| :--- | :--- |
| **Nombre completo** | `[Vladimir Sebastian Acelas Rodriguez]` |
| **Sistema operativo** | Windows `[11]` |
| **Fecha** | `[17/06/2026]` |

---

## Proceso de Instalación

El proceso se realizó en tres fases principales:

1. **Descarga:** Se descargó el *MySQL Installer for Windows* desde el sitio oficial de MySQL Community Downloads.
2. **Configuración de credenciales:** Durante la instalación se configuró el servidor en modo *Development Computer* (puerto 3306) y se definió la contraseña del usuario `root`, encargado de administrar el servidor.
3. **Finalización:** Se aplicó la configuración, se instaló MySQL Workbench y se verificó la conexión al servidor local mediante la conexión *Local Instance*.

---

## Galería de Evidencias

### Captura 1 — Instalación / Descarga completada
![Instalador de MySQL en ejecución](imagenes_MySQL/Instalador de MySQL en ejecución.png)

### Captura 2 — Configuración de la contraseña del usuario root
![Configuración de credenciales del usuario root](imagenes_MySQL/Configuración de credenciales del usuario root.png)

### Captura 3 — MySQL Workbench con la conexión Local Instance
![MySQL Workbench con la conexión Local Instance creada](imagenes_MySQL/MySQL Workbench con la conexión Local Instance creada.png)

---

## Validación del Entorno

Para confirmar que la instalación fue exitosa, se ejecutó la siguiente consulta en una pestaña **Query** de MySQL Workbench:

```sql
-- Consulta de validación de entorno
SELECT VERSION() AS 'Versión de MySQL', 
       CURRENT_USER() AS 'Usuario Actual', 
       NOW() AS 'Fecha y Hora del Servidor';
```

El resultado confirma la **versión de MySQL** instalada, el **usuario** conectado y la **fecha y hora** del servidor:

![Resultado de la consulta de validación](imagenes_MySQL/Resultado de la consulta de validación.png)
