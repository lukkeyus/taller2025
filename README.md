# Taller de Administración en Servidores Linux (Julio–Agosto 2025)

## Entorno de práctica

Se utilizarán **tres máquinas virtuales**:

1. **Bastión — CentOS Stream 9 (con interfaz gráfica)**
   - VM con entorno gráfico.
   - Se usará para conectarse por **SSH** al resto de las VMs.

2. **Nodo 1 — CentOS Stream 9 (instalación mínima)**

3. **Nodo 2 — Ubuntu 24.04 LTS (instalación mínima)**

## Usuario y acceso

- Usuario común en todas las VMs: `sysadmin`.
- Acceso por **SSH con clave pública** (la clave del bastión se copia a cada nodo).
- `sysadmin` está en **sudoers** con privilegios de administración

## Instrucciones de uso 


