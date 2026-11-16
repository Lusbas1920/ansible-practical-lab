# Laboratorio práctico de Ansible con Docker

## 1. Descripción del proyecto

Este proyecto consiste en implementar un laboratorio práctico de automatización utilizando Ansible y Docker.

Se utilizan dos contenedores Ubuntu como servidores administrados, desde los cuales se ejecutan tareas automatizadas mediante un playbook de Ansible.

## 2. Tecnologías utilizadas

- Ubuntu
- Docker
- Docker Compose
- Ansible
- YAML
- Git y GitHub

## 3. Estructura del proyecto

```text
ansible-practical-lab/
├── docker-compose.yml
├── inventory.ini
├── playbook.yml
└── README.md
```

## 4. Configuración del laboratorio

Se crearon dos servidores Docker:

- ansible-servidor1
- ansible-servidor2

Ambos utilizan la imagen `ubuntu:latest` y permanecen activos para recibir instrucciones de Ansible.

Se configuraron servidores DNS para permitir que los contenedores accedan a los repositorios de Ubuntu.

## 5. Inventario de Ansible

El archivo `inventory.ini` contiene los dos servidores y utiliza el complemento de conexión Docker de Ansible.

## 6. Tareas automatizadas

El archivo `playbook.yml` realiza las siguientes operaciones:

1. Recopilar información de los servidores.
