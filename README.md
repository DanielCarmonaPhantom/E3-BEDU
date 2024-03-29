<img src='./src/img/Titular.png'>

# E3-BEDU
![Django](https://img.shields.io/static/v1?style=for-the-badge&message=Django&color=092E20&logo=Django&logoColor=FFFFFF&label=)
![DOCKER](https://img.shields.io/badge/docker-14354C?style=for-the-badge&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/static/v1?style=for-the-badge&message=PostgreSQL&color=4169E1&logo=PostgreSQL&logoColor=FFFFFF&label=)
![Bootstrap](https://img.shields.io/badge/bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)


------
## Proyecto Final de Módulo Django
   
### Introducción:
El E3 es un evento que se realizaba anteriormente de forma presencial. Al llegar la pandemia, tuvo que ser cancelado como muchos eventos. 

### Objetivo:
Diseñar un sitio web donde se pueda realizar el evento. Al intercambiar el modo presencial a en línea, se busca de alguna manera, seguir teniendo esa interacción con los usuarios.

### Arquitectura del proyecto

1. Problemnt Statement e Investigación de Usario
2. Docker y Postgresql para la base de datos
3. Proyecto realizado con Django
4. Diseño Ui de la interfaz de Usuario
5. Demo de Proyecto


<section>
  <h3>1. Problemnt Statement e Investigación de Usario</h3>
  
  <p>A partir de la investigación, obtuvimos para la arquitectura de nuestro sitio el siguiente esquema:</p>

  <ul>
    <li>Home</li>
    <li>Login</li>
    <li>Dashboard</li>
    <li>Stands</li>
    <li>Articulos</li>
  </ul>

  <p>Se diseñaron wireframes de baja fidelidad donde se plasmaba los procesos que se habían obtenido de la investigación:
  <img src='./src/img/Low.png'>
</section>

<section id="docker">
  <h3>2. Docker y Postgresql para la base de datos</h3>
  <p>Se trabajo con instancias de Docker para ejecutar Postgresql</p>
  <p>Se trabajaron 3 modelos</p>  
  <img src='./src/img/Diagrama.png'> 
</section>

<section id="backend">
  <h3>3. Proyecto realizado con Django</h3>
  <p>Se empezo levantando el proyecto de Cokiecutter Django</p>
  <p>Para hacer el inicio de sesión y registro trabajamos con las loginview</p>
  <p>Se realizaron 4 apps dentro del proyecto</p>  
  <img src='./src/img/Proyecto.png'> 
</section>


 
<section id="uid">
  <h3>4. Diseño Ui de la interfaz de Usuario</h3>
   
  <p>Se empezo todo el proceso de diseño donde a partir de un moodboard y un style guide, se trabajó en los prototipos de alta fidelidad</p>   
  <img src='./src/img/Home.png'>
  <img src='./src/img/Login.png'>
  <img src='./src/img/Register.png'>
  <img src='./src/img/Dashboard.png'>
  <img src='./src/img/Modal.png'>
  <img src='./src/img/Stand.png'>
</section>

<section id="uid">
  <h3>5. Demo del Proyecto</h3>
   <p>Se hará un Live Demo desde la página de home, haciendo un login de usuario, se visualizará el dashboard y herramientas, y finalizando con un post a los stands.</p>   
   <img src='./src/img/LiveDemo.png'> 
</section>

Gracias.

```
< PROJECT ROOT >
   |
   |-- core/                               # Implements app logic and serve the static assets
   |    |-- settings.py                    # Django app bootstrapper
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |-- templates/                     # Templates used to render pages
   |         |
   |         |-- includes/                 # HTML chunks and components
   |         |-- layouts/                  # Master pages
   |         |-- accounts/                 # Authentication pages
   |         |
   |      index.html                       # The default page
   |       *.html                          # All other HTML pages
   |
   |-- authentication/                     # Handles auth routes (login and register)
   |    |-- urls.py                        # Define authentication routes  
   |    |-- forms.py                       # Define auth forms  
   |
   |-- app/                                # A simple app that serve HTML files
   |    |-- views.py                       # Serve HTML pages for authenticated users
   |    |-- urls.py                        # Define some super simple routes  
   |
   |-- customers/                          # Handles the profile edit     <-------- NEW
   |    |-- __init__.py                    # Defines App init             <-------- NEW
   |    |-- admin.py                       # Defines App admin            <-------- NEW
   |    |-- apps.py                        # Defines App apps             <-------- NEW
   |    |-- forms.py                       # Defines App forms            <-------- NEW
   |    |-- models.py                      # Defines App models           <-------- NEW
   |    |-- signals.py                     # Defines App signals          <-------- NEW
   |    |-- tests.py                       # Defines App tests            <-------- NEW
   |    |-- urls.py                        # Defines App routes           <-------- NEW
   |    |-- views.py                       # Defines App views            <-------- NEW
   |
   |-- requirements.txt                    # Development modules - SQLite storage
   |-- .env                                # Inject Configuration via Environment
   |-- manage.py                           # Start the app - Django default start script
   |
   |-- ************************************************************************
```  
