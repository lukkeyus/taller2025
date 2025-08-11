ORT Cuestionario del Taller de Administración en Servidores Linux Julio-Agosto 2025



Lucas Gómez 310745 y Caetano Ferres 327646.



1\. Ansible es una herramienta de automatización basado en Python que nos permite automatizar tareas repetitivas y/o complejas. 2 de las tareas mas comunes que podemos realizar con ansible son la creación y configuración de servidores virtuales y el automatizar la aplicación de parches y actualización en nuestros sistemas.



2\. Un playbook de ansible es un archivo YAML el cual define las tareas de automatización a realizar, es básicamente una guía que ansible debe ejecutar para realizar la tarea que nosotros como sysadmin le comandamos.



3\. Un inventario de Ansible debe contener información sobre los hosts (los servidores que gestiona), datos como su dirección IP, su host name, el grupo de hosts al que pertenece y alguna variable especifica del host, como un usuario o puerto del servidor.



4\. Un modulo de Ansible  es un programa que lleva a cabo tareas ya sea en un equipo local, en una API o en un host remoto. Los módulos se expresan como código y contienen metadatos que definen el momento y el lugar en el que se ejecuta una tarea de automatización, uno de los módulos que se incluyen con Ansible Core (es decir forman parte de todas las instalaciones de Ansible) es el modulo dnf, este instala, actualiza y elimina los paquetes y los grupos con dnf, el cual es el gestor de paquetes de software predeterminado de las distribuciones tipo CentOS (a partir de CentOS 8).



5\. Ansible destaca sobre todo por su simplicidad, dado a que al estar escrito en YAML nos resulta mucho mas simple y ameno a la hora de leerlo a diferencia de lenguajes como JSON, por ejemplo.



Fuentes: **Ansible: ¿Qué es y cómo funciona?:** https://www.redhat.com/es/topics/automation/learning-ansible-tutorial

         **Módulos de Ansible: qué son y cómo funcionan:** https://www.redhat.com/es/topics/automation-and-management/modulos-de-ansible-que-son-y-como-funcionan

