# proyectoDFS
<p align="center">
<img src="varios/logos.png" width="300"
</p>

---
Plantilla desarrollada en HTML5, CSS3

Archivos principales:
---
- index.html
- identidad.html
- portafolio.html
- cvu.html
- acerca.html

Estructura de la plantilla:
---
/--
  |- css .- Hojas de estilo para las páginas html
  |- img .- Imagenes utilizadas en las páginas html
  |- varios .- Archivos para el diseño de readme.
  
# Proyecto Web Personal — Control de Versiones con Git y GitHub

Repositorio desarrollado como parte de las prácticas de laboratorio de control de versiones. Este proyecto integra la estructura de un sitio web estático modular y documenta los comandos de Git utilizados.

---

##  Estructura del Proyecto

El sitio web está compuesto por las siguientes páginas y carpetas:

* `index.html`: Página principal con menú horizontal y tabla central de navegación.
* `identidad.html`: Sección personal con fotografía.
* `portafolio.html`: Resumen de trabajos y proyectos realizados.
* `cvu.html`: Datos de currículum vitae y habilidades técnicas.
* `acerca.html`: Información de perfil y áreas de interés.
* `css/`: Hoja de estilos `style.css` para el centrado del contenido y presentación general.
* `img/`: Recursos gráficos del sitio (`cvu.jpg`, `identidad.jpg`, `portafolio.jpg`, `foto.jpg`).

---

## Comandos de Git Utilizados

### 1. Configuración Inicial y Entorno Local
| Comando | Descripción |
| :--- | :--- |
| `git config --list` | Muestra la configuración actual de Git en el equipo. |
| `git config --global user.name "Nombre"` | Registra el nombre de autor para las confirmaciones. |
| `git config --global user.email "correo"` | Registra el correo asociado a los commits y a GitHub. |
| `git init` | Inicializa un nuevo repositorio Git en el directorio de trabajo actual. |

### 2. Ciclo Básico de Trabajo y Confirmaciones
| Comando | Descripción |
| :--- | :--- |
| `git status` | Consulta el estado actual de los archivos (modificados, en staged o no rastreados). |
| `git add .` | Agrega todos los archivos nuevos y modificados al área de preparación (*staged*). |
| `git add <archivo>` | Agrega un archivo puntual al área de preparación (*staged*). |
| `git commit -m "mensaje"` | Confirma y guarda permanentemente los cambios en el historial local. |

### 3. Inspección de Historial y Versiones
| Comando | Descripción |
| :--- | :--- |
| `git log` | Despliega el historial de confirmaciones registradas. |
| `git log --oneline` | Muestra el historial resumido a un renglón por commit. |
| `git log --stat` | Lista los commits junto con las estadísticas de archivos alterados. |
| `git show <archivo>` | Inspecciona en detalle las modificaciones del último commit sobre un archivo. |
| `git diff <hash1> <hash2>` | Muestra las diferencias línea por línea entre dos versiones del repositorio. |
| `git checkout <hash> -- <archivo>` | Revierte un archivo al estado exacto que poseía en un commit previo. |

### 4. Gestión de Ramas (*Branching*) y Fusión
| Comando | Descripción |
| :--- | :--- |
| `git branch` | Lista las ramas locales e indica cuál está activa con un asterisco. |
| `git branch <nombre>` | Crea una nueva rama de trabajo. |
| `git branch -m main` | Renombra la rama actual (usada para cambiar `master` a `main`). |
| `git checkout <nombre>` | Cambia el espacio de trabajo hacia la rama indicada. |
| `git merge <rama>` | Integra los commits y modificaciones de la rama indicada en la rama activa. |

### 5. Conexión Remota y Llaves SSH con GitHub
| Comando | Descripción |
| :--- | :--- |
| `ssh-keygen -t rsa -b 4096 -C "correo"` | Genera un par de llaves criptográficas asimétricas (pública y privada). |
| `eval $(ssh-agent -s)` | Inicia el proceso del agente SSH en segundo plano. |
| `ssh-add id_rsa` | Registra la llave privada en el agente SSH de la máquina local. |
| `ssh -T git@github.com` | Valida la conexión y autenticación criptográfica con GitHub. |
| `git remote add origin <url>` | Enlaza el repositorio local con un repositorio remoto en GitHub. |
| `git remote -v` | Muestra las direcciones configuradas para el envío y recepción de cambios. |
| `git remote set-url origin <url_ssh>` | Modifica la URL del repositorio remoto para usar autenticación SSH. |
| `git pull origin main --allow-unrelated-histories` | Descarga y fusiona historias iniciales independientes entre el repositorio local y el remoto. |
| `git push origin main` | Publica las confirmaciones de la rama local hacia el repositorio remoto en GitHub. |

---

## Autor
* **Diego Fernando Domínguez Sánchez**
* **Instituto Tecnológico de Villahermosa (TecNM)**
