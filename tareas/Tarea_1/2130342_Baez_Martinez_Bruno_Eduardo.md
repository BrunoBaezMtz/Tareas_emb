
# *Comandos básicos de PowerShell*

## Cambiar de directorio

### `cd`

se usa para cambiar el directorio (carpeta) de trabajo actual.

---

## Ejemplo de uso

```powershell
# Ir a la carpeta C:\Documentos
cd C:\Documentos

# Regresar una carpeta
cd ..

# Ir a una carpeta especifica 
cd C:\Program Files\Mi App

```

## Listar contenido

### `ls` 
    
muestra una lista de los archivos y carpetas en el directorio actual o en una ruta especificada.

---

```powershell
# Listar contenido del directorio actual
ls

# Listar contenido de otra carpeta
ls C:\Users\Publico

# Listar incluyendo archivos ocultos (-Force)
ls -Force

```
## Crear directorio
### `mkdir`
se utiliza para crear una nueva carpeta.

---
```powershell
# Crear una carpeta en la ubicación actual
mkdir ProyectoNuevo

# Crear una carpeta en una ruta específica
mkdir C:\Temp\Reportes
```

## Limpiar pantalla
### `clear` 
limpia todo el texto de la consola, dejando un prompt limpio en la parte superior.

---

```powershell
# Limpia la terminal
clear
```

## Mostrar directorio actual
### `pwd`
significa "Print Working Directory" (Imprimir Directorio de Trabajo). Muestra la ruta completa del directorio actual.

---

```powershell
# Muestra dónde estás ahora
pwd

# Output: C:\Users\TuUsuario\Documentos
```

## Mostrar contenido de archivo
### `cat`
se usa para leer el contenido de uno o más archivos y mostrarlo en la consola.

---

```powershell
# Mostrar el contenido de un archivo de texto
cat C:\Temp\log.txt

# Mostrar las primeras 10 líneas de un archivo
cat .\mi_script.ps1 -TotalCount 10
```

## Copiar archivos
### `cp` 
copia uno o más archivos o carpetas de una ubicación a otra.

---

```powershell
# Copiar un archivo a otra carpeta
cp .\archivo.txt C:\Backup\

# Copiar una carpeta entera
cp .\Proyecto -Destination C:\Archivo
```

## mover o renombrar
### `mv`
mueve un archivo o carpeta a una nueva ubicación. También se usa para renombrar ítems.

---

```powershell
# Mover un archivo a otra carpeta
mv .\reporte.pdf C:\ReportesFinales\

# Renombrar un archivo (moverlo a la misma carpeta con otro nombre)
mv .\viejo_nombre.txt .\nuevo_nombre.txt
```

# *Comandos básicos de Git*

## Inicializar repositorio
### `git init`
Crea un nuevo repositorio de Git vacío en el directorio actual. Genera la subcarpeta oculta .git que rastrea los cambios.

---

```powershell
# Inicializa el directorio actual como un repositorio Git
git init
```

## Clonar repositorio 
### `git clone`
Descarga una copia (un "clon") de un repositorio remoto existente (ej. de GitHub) a una nueva carpeta local.

---

```powershell
# Clona un repositorio desde una URL
git clone [https://github.com/usuario/proyecto.git](https://github.com/usuario/proyecto.git)
```

## Ver diferencias
### `git diff`
Muestra las diferencias entre los archivos modificados en el directorio de trabajo y el último commit (o entre dos commits/ramas).

---

```powershell
# Muestra cambios no "stageados" (no agregados)
git diff

# Muestra cambios "stageados" (agregados con 'add')
git diff --staged
```

## Ver estatus
### `git status`
Muestra el estado del directorio de trabajo: qué archivos están modificados, cuáles están en "staging" (listos para commit) y cuáles no están siendo rastreados.

---

```powershell
# Revisa el estado actual del repositorio
git status
```

## Fusionar ramas
### `git merge`
Combina los cambios de una rama (ej. "feature") en la rama actual (ej. "main"). Resuelve las historias de commits en una sola.

---

```powershell
# Estando en la rama 'main', fusiona los cambios de 'nueva-feature'
git checkout main
git merge nueva-feature
```

## Configurar git
### `git config`
Se usa para establecer o ver las variables de configuración de Git (a nivel de usuario, global o de repositorio).

---

```powershell
# Configurar tu nombre de usuario globalmente
git config --global user.name "Tu Nombre"

# Configurar tu email globalmente
git config --global user.email "tu@email.com"
```

## Agregar al staging
### `git add`
Agrega los cambios de los archivos al área de "staging" (preparación), indicando que esos cambios específicos se incluirán en el próximo commit.

---

```powershell
# Agregar un archivo específico
git add tarea-_-1

# Agregar todos los archivos modificados y nuevos
git add -A
```

## Ver historial
### `git log`
Muestra el historial de commits del repositorio, listando el autor, fecha y mensaje de cada commit.

---

```powershell
# Muestra el historial completo
git log

# Muestra un historial resumido en una línea
git log --oneline
```

## Guardar cambios
### `git commit`
Guarda permanentemente los cambios que están en el "staging area" en el historial del repositorio, creando una nueva "instantánea" (commit) con un mensaje descriptivo.

---

```powershell
# Realiza un commit con un mensaje
git commit -m "Agrega la página de contacto"
```

## Cambiar de rama o deshacer
### `git checkout`
Se usa principalmente para cambiar entre diferentes ramas. También puede usarse para descartar cambios en un archivo.

---

```powershell
# Cambiar a una rama existente
git checkout main

# Crear y cambiar a una nueva rama
git checkout -b nueva-feature

# Descartar cambios en un archivo (volver al último commit)
git checkout -- mi_archivo.txt
```

## Administrar ramas
### `git branch`
Permite listar, crear o eliminar ramas (versiones paralelas del historial de trabajo).

---

```powershell
# Listar todas las ramas locales
git branch

# Crear una nueva rama
git branch feature/login

# Eliminar una rama
git branch -d rama-obsoleta
```

## Traer y fusionar
### `git pull`
Actualiza el repositorio local trayendo los cambios del repositorio remoto y automáticamente los fusiona (merge) en la rama local actual.

---

```powershell
# Actualiza la rama actual desde el remoto 'origin'
git pull origin main
```

## Subir cambios
### `git push`
Envía los commits locales (que no están en el remoto) al repositorio remoto (ej. GitHub), actualizándolo.

---

```powershell
# Sube los commits de la rama 'main' al remoto 'origin'
git push origin main
```

## Traer cambios (sin fusionar)
### `git fetch`
Descarga los cambios (nuevos commits, ramas, etc.) del repositorio remoto, pero no los fusiona automáticamente en el trabajo local. Permite revisar los cambios antes de integrarlos.

---

```powershell
# Trae todas las actualizaciones del remoto 'origin'
git fetch origin
```

# *Proceso para crear un repositorio de Git desde PowerShell*

## 1. Crear carpeta y entrar en ella
Primero, usamos los comandos de PowerShell para crear el directorio donde vivirá el proyecto y luego navegamos hacia él.

---

```powershell
# Creamos una nueva carpeta llamada "MiProyecto"
mkdir MiProyecto

# Entramos en la carpeta recién creada
cd MiProyecto
```

## 2. Inicializar el repositorio
Una vez dentro de la carpeta del proyecto, usamos Git para convertirla en un repositorio.

---

```powershell
# Inicializa Git en la carpeta actual
git init
```

## 3. Agregar archivos al Staging Area
Ahora, crea o agrega los archivos de tu proyecto a esta carpeta (por ejemplo, README.md). Una vez que los archivos existen, debes indicarle a Git que quieres rastrearlos usando git add.

---

```powershell
# Agrega TODOS los archivos nuevos y modificados al "staging"
git add -A

# Si solo quisieras agregar un archivo:
# git add README.md
```

## 4. Realizar un primer commit
Finalmente, guarda esta primera "instantánea" de tu proyecto en el historial de Git. Este es tu primer commit.

---

```powershell
# Guarda los archivos del staging en el historial
git commit -m "Commit inicial: Creación del proyecto"
```

