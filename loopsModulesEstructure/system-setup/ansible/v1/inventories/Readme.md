donde escribo host estaticos, host dinamicos, archivos de configuracion para cada ambiente o archivo de configuracion para cada aplicacion
- direcciones ip en hosts, se ejecuta un playbook por aplicacion y se identifica por el hosts a quien se lo va a plicar

prod:
- hosts.static: se usa para escribir inventarios estaticos
para definirlo debo crear un grupo
- inventory_aws_ec2: dinamicos
- group_vars : 
  - carpetas con nombre de los procesos ejm: app1 y app2 : en cada una se guardan las variables para cada aplicación
  - la carpeta all es obligatoria