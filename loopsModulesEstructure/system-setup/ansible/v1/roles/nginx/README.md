Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

----------------------
default : en main.yaml se definen todas las variables del rol con un valor por defecto y que pueden ser dinamicas, es con un archivo de inputs
files : se usa cuando se necesita subir archivos o modificar archivos en la automatizacion
meta : donde le doy la información del rol
task : donde se definen las tareas definidas como un array y llama por defecto al main.yml
templates : se crean todos los archivos de tipo template con la herramienta jinja y jinja2 https://jinja.palletsprojects.com/en/3.1.x/, ansible no es nada mas que configuracion y quien hace la magia es python por ende si necesitamos pregenerar archivos en base a variables de entorno necesitamos un template. y jinja ese l formato de template para python
un template es un arcihvo base que tiene la esructura para crear un archivo con variables dinamicas, la salida es un archivo final
test : prubas unitarias para ansible y se pueden levantar instancias efimeras
vars : se definen constantes, no se pueden modificar, se usan en la ejecucion del modulo para parsear archivos