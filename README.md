# Proyecto de Gestión de Negocio - Django

Este proyecto consiste en una aplicación web desarrollada con **Django** para la gestión de inventario, permitiendo administrar categorías y productos de forma relacional.

## Características del Proyecto
* **Gestión de Categorías**: Permite agrupar productos (ej: Zapatillas, Electrónica).
* **Gestión de Productos**: Registro de artículos con nombre, precio, stock y categoría asociada.
* **Panel de Administración**: Interfaz completa (CRUD) para Crear, Leer, Actualizar y Borrar datos de forma visual.
* **Base de Datos Relacional**: Uso de `ForeignKey` para conectar productos con sus respectivas categorías.

##  Problemas Encontrados y Soluciones
Durante el desarrollo surgieron varios desafíos técnicos que fueron superados:
1. **Permisos de Administrador (sudo)**: Al intentar crear el entorno virtual, hubo conflictos de permisos en el sistema Linux. Se solucionó instalando las dependencias a nivel de usuario y configurando el proyecto directamente en la carpeta local.
2. **Configuración de Aplicaciones**: Fue necesario registrar manualmente la app `gestion` en el archivo `settings.py` para que Django reconociera los modelos.
3. **Autenticación en GitHub**: Debido a las políticas de seguridad actuales, la subida del código requirió la generación de un **Personal Access Token (classic)** en lugar de la contraseña convencional.

##  Cómo ejecutar el proyecto
1. Clonar el repositorio: `git clone https://github.com/repo819-eng/ProyectoNegocio.git`
2. Instalar Django: `pip install django`
3. Ejecutar migraciones: `python3 manage.py migrate`
4. Crear superusuario: `python3 manage.py createsuperuser`
5. Iniciar servidor: `python3 manage.py runserver`

## Acceso al Panel de Administración

Para gestionar el inventario, utiliza las siguientes credenciales en http://127.0.0.1:8000/admin:
Usuario: admin
Contraseña: admin

## Análisis y Evaluación Personal

El desarrollo de esta aplicación ha permitido entender cómo Django facilita la creación de sistemas de gestión mediante su panel de administración y su ORM relacional.

Aunque el proceso tomó más tiempo del previsto debido a la configuración del entorno en Linux y la gestión de permisos, el resultado es una herramienta funcional que cumple con los requisitos de un CRUD relacional. He aprendido la importancia de gestionar correctamente los entornos virtuales y las dependencias (requirements.txt) para asegurar que el proyecto sea reproducible en cualquier máquina.
