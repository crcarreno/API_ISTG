# Requerimientos
Ubuntu 16 o superior

Python 3.6.3

# Instalar librerías
python3.6 -m pip -r install requirements.txt

# GIT 
git pull origin

En caso de conflictos
git stash

# Iniciar el proyecto

Cambiar los parámetros de base de datos para que funciones desde el servidor

python3.6 -m pip install gunicorn

gunicorn -w 4 -b 0.0.0.0:5000 app:app

# Crear servicio para arrancar el proyecto con el gunicorn
Utilizar el archivo start.sh

Habilitar permisos de ejecución chmod +x start.sh

Crear servicio utilizando el archivo make_service 

# Modo Developer

Instalar Python 3.6.3

# Ingresar a la carpeta virtual
source .venv/bin/activate

# Salir
deactivate

# Activar el .venv ejecutar
pip install flask

pip freeze > requirements.txt

# Instalar librerías

# Test
http://localhost:5000/estudiante?cedula=0958476533&sede=GYE

http://localhost:5000/asistencia?cedula=0958476533&date_ini=2024-01-01&date_end=2024-01-30'