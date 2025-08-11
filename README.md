# Taller de Administración en Servidores Linux (Julio–Agosto 2025)

## Entorno de práctica

Se utilizarán **tres máquinas virtuales**:

1. **Bastión - CentOS Stream 9 (con interfaz gráfica)**
   - VM con entorno gráfico.
   - Se usará para conectarse por **SSH** al resto de las VMs.

2. **Nodo 1 - CentOS Stream 9 (instalación mínima)**

3. **Nodo 2 - Ubuntu 24.04 LTS (instalación mínima)**

## Usuario y acceso

- Usuario común en todas las VMs: `sysadmin`.
- Acceso por **SSH con clave pública** (la clave del bastión se copia a cada nodo).
- `sysadmin` está en **sudoers** con privilegios de administración

## Instrucciones de uso 

**Pre-requisitos: Contar con una estructura de maquinas virtuales similar al entorno de practica**

**1 - Clonar el repositorio**

   Para obtener los archivos necesario para la ejecucion de los playbooks vamos a clonar los repositorios en nuestro bastion.
Para ello usamos `git clone https://github.com/lukkeyus/taller2025.git`

Luego de eso vamos hacia el directorio

`cd taller2025`

**2 - Instalar colecciones necesarias**

Esto incluye librerias y paquetes necesarios.
Ejecutamos el comando: `ansible-galaxy collection install -r requirements.yml

**3 - Configuracion del inventario**

   Si nuestro entorno difiere en cantidad de maquinas o configuracion de red tendras que editar `inventory.ini` con tus IPs o lista de maquinas reales.
Tambien puede variar el usuario con el que haces login ssh (Ejemplo de nuestro caso usamos `sysadmin)

Opcional: Se puede verificar la conexion sin contraseña

`ssh USUARIO@IP_VM`

Si solicita la clave del usuario es que no esta cargada la clave publica. Esto se puede solventar con 

`ssh-copy-id*USUARIO@IP-VM`

**4 - Prueba de conectividad**

Para probar la conectividad con los hosts configurados

`ansible all -i inventory.ini -m ping`

**5 - Playbook NFS**

Este playbook instala el servicio de NFS en el host que definamos como webserver.

Para ejecutarlo usamos: `ansible-playbook -i inventory.ini playbooks/nfs_setup.yml`

**6 - Playbook hardening (enfocado a Ubuntu**

Similar a lo anterior, para ejecutrar este playbook utilizamos el siguiente comando:

`ansible-playbook -i inventory.ini playbooks/hardening.yml`



