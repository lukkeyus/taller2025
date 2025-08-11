## ORT — Cuestionario del Taller de Administración en Servidores Linux (Julio–Agosto 2025)

**Autores:** Lucas Gómez (310745) y Caetano Ferres (327646)

## Preguntas y respuestas

1. **¿Qué es Ansible? Mencione dos actividades que se puedan hacer con Ansible**  
   Ansible es una herramienta de automatización basada en Python que permite automatizar tareas repetitivas y/o complejas. Dos tareas comunes son:
   - Creación y configuración de servidores virtuales.
   - Automatización de la aplicación de parches y actualizaciones en los sistemas.

2. **¿Qué es un playbook de Ansible?**  
   Un playbook de Ansible es un archivo YAML que define las tareas de automatización a realizar; es básicamente la guía que Ansible ejecuta para cumplir lo que nosotros como sysadmins definimos.

3. **¿Que información contiene un inventario de Ansible?**  
   Debe incluir información de los hosts gestionados: dirección IP, hostname, grupos de hosts y variables específicas del host (por ejemplo, usuario o puerto SSH).

4. **Explique que es un módulo de Ansible y dé un ejemplo.**  
   Un modulo de Ansible  es un programa que lleva a cabo tareas ya sea en un equipo local, en una API o en un host remoto. Los módulos se expresan como código y contienen metadatos que definen el momento y el lugar en el que se ejecuta una tarea de automatización, uno de los módulos que se incluyen con Ansible Core (es decir forman parte de todas las instalaciones de Ansible) es el modulo dnf, este instala, actualiza y elimina los paquetes y los grupos con dnf, el cual es el gestor de paquetes de software predeterminado de las distribuciones tipo CentOS (a partir de CentOS 8)

5. **¿Que ventajas tiene Ansible sobre otros métodos de automatización?**  
   Ansible destaca sobre todo por su simplicidad, dado a que al estar escrito en YAML nos resulta mucho mas simple y ameno a la hora de leerlo a diferencia de lenguajes como JSON, por ejemplo.

## Fuentes

- [Ansible: ¿Qué es y cómo funciona? — Red Hat](https://www.redhat.com/es/topics/automation/learning-ansible-tutorial)  
- [Módulos de Ansible: qué son y cómo funcionan — Red Hat](https://www.redhat.com/es/topics/automation-and-management/modulos-de-ansible-que-son-y-como-funcionan)
