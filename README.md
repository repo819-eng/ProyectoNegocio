# 🚀 Proyecto de Gestión de Negocio - Django

Este proyecto consiste en una aplicación web desarrollada con **Django** para la gestión de inventario de un negocio de calzado, permitiendo administrar categorías y productos de forma relacional.

---

## 🛠️ 1. Herramientas utilizadas y provadas
Para el desarrollo de esta aplicación se han utilizado y testeado las siguientes tecnologías:
* **Lenguaje:** Python 3.10
* **Framework:** Django 5.x
* **Base de Datos:** SQLite (motor relacional por defecto de Django)
* **Control de Versiones:** Git y GitHub
* **Entorno de desarrollo:** Terminal de Linux (Ubuntu/Debian) y VS Code
* **Gestión de Dependencias:** pip y archivo `requirements.txt`

---

## 🏗️ 2. Proceso de creación del código
El desarrollo se ha realizado siguiendo estos pasos técnicos:
1. **Inicialización:** Creación del proyecto base y la aplicación `gestion`.
2. **Modelado de Datos:** Definición de la relación $1:N$ entre las entidades `Categoria` y `Producte` mediante `ForeignKey`.
3. **Persistencia:** Ejecución de migraciones con `makemigrations` y `migrate` para generar las tablas en SQLite.
4. **Interfaz Administrativa:** Registro de modelos en `admin.py` para habilitar un sistema CRUD (Create, Read, Update, Delete) completo y funcional.
5. **Pruebas:** Carga de datos reales (Zapatillas) para validar la integridad de la base de datos.

---

## 📦 3. Instrucciones de instalación
Siga estos pasos para ejecutar el proyecto en su máquina local:

**Clonar el repositorio:**
git clone [https://github.com/repo819-eng/ProyectoNegocio.git](https://github.com/repo819-eng/ProyectoNegocio.git)
cd ProyectoNegocio
   
Instalar dependencias:
pip install -r requirements.txt

Preparar la Base de Datos:
python3 manage.py migrate

Iniciar el servidor:
python3 manage.py runserver

## Acceso al CRUD:
Entre en http://127.0.0.1:8000/admin con las siguientes credenciales:

## Usuario: admin
## Contraseña: admin

## 4. Dificultades encontradas

Durante el proceso surgieron varios desafíos técnicos que fueron superados con éxito:
    Entornos Virtuales en Linux: Conflictos de permisos (sudo) al intentar crear el venv. Se solucionó instalando dependencias a nivel de usuario.
    Seguridad de GitHub: La necesidad de generar un Personal Access Token (classic) para poder realizar push desde la terminal de Linux debido a las políticas actuales de Git.
    Módulos de Django: Errores de importación solucionados registrando correctamente la app en settings.py.

## 5. Análisis y evaluación personal

La aplicación cumple con todos los objetivos propuestos: es funcional, reproducible y gestiona datos relacionales.

## Valoración final:
A pesar de las dificultades iniciales con la terminal de Linux y el tiempo invertido en la configuración de Git, la experiencia ha servido para comprender el flujo de trabajo real de un desarrollador: desde la lógica de base de datos hasta el despliegue en un repositorio público. El uso de la IA y la documentación oficial de Django han sido clave para resolver errores rápidamente.
