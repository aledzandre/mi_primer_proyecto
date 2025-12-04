
PASO 1: Configurar Git (solo una vez por computadora)
Abre Visual Studio Code, abre la terminal (Ctrl + ñ o Ctrl + `) y escribe:
git config --global user.name "Jhon Martinez"
git config --global user.email aledzandre@gmail.com

Verifica tu configuración:
git config –list

PASO 2: Crear el proyecto
Crea una carpeta para tu proyecto:
mkdir mi_primer_proyecto
cd mi_primer_proyecto
Inicializa Git en la carpeta:
git init

PASO 3: Crear el script en Python
Usando Visual Studio Code crea el archivo hola.py y escribe el siguiente código:
# hola.py
# Autor: (tu nombre)
# Descripción: Script básico que saluda al usuario
nombre = input("¿Cómo te llamas? ")
print(f"¡Hola, {nombre}! Bienvenido a tu primer proyecto con Git y Python.")

PASO 4: Ver el estado del repositorio
git status
PASO 5: Agregar archivos al área de preparación O todos los archivos:
git add hola.py

PASO 6: Crear el primer commit
git commit -m "Primer commit: script de saludo en Python"
 
PASO 7: Crear el repositorio en GitHub
1. Entra a https://github.com
2. Clic en New repository
3. Nómbralo mi_primer_proyecto
4. No marques “Initialize with README”
5. Crea el repositorio y copia la URL HTTPS

PASO 8: Conectar el repositorio local con GitHub
git remote add origin https://github.com/aledzandre/mi_primer_proyecto.git
git remote -v

PASO 9: Subir los archivos a GitHub
git branch -M main
git push -u origin main

PASO 10: Hacer cambios y subir una nueva versión
Contenido del archivo hola.py
# hola.py
# Versión mejorada
nombre = input("¿Cómo te llamas? ")
print(f"¡Hola, {nombre}! Bienvenido a tu primer proyecto con Git y Python.")
print(f"Tu nombre tiene {len(nombre)} letras.")

Guarda y ejecuta:
git status
git add hola.py
git commit -m "Segunda versión: se muestra la longitud del nombre"
git push
 
