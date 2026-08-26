# Eduardo Sánchez

**Ingeniero de Software Senior — Infraestructura Cloud y Seguridad**

10+ años construyendo y asegurando sistemas en producción: arquitectura AWS, CI/CD, hardening de servidores Linux y aplicaciones full-stack para banca, salud y gobierno.

🌐 [Portafolio](https://eduarsb.github.io) · 🛠️ [DawnForge](https://www.dawnforge.xyz) · ✉️ [eduarsb4@gmail.com](mailto:eduarsb4@gmail.com)

### Stack

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat&logo=amazon-aws&logoColor=white)
![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=flat&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/linux-%23FCC624.svg?style=flat&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=flat&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=flat&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/jenkins-%232C5263.svg?style=flat&logo=jenkins&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=flat&logo=laravel&logoColor=white)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=flat&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)
![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=flat&logo=angular&logoColor=white)
![Vue.js](https://img.shields.io/badge/vue.js-%2335495e.svg?style=flat&logo=vuedotjs&logoColor=%234FC08D)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat&logo=typescript&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=flat&logo=mysql&logoColor=white)

### Proyectos destacados

**[aws-reference-stack](https://github.com/eduarsb/aws-reference-stack)** — Arquitectura AWS pequeña pero con forma de producción, descrita entera en Terraform: servicio web en contenedores detrás de un ALB y una tubería de trabajo asíncrono, unidas con IAM de mínimo privilegio. Se despliega con `terraform apply` y nada más.

Tres decisiones que muestra, y que también hay que tomar en un sistema real:

- Red en dos zonas de disponibilidad, con el cómputo en subredes privadas y salida por un único NAT gateway.
- Cola de trabajos con cola de mensajes muertos tras tres fallos, para que un mensaje envenenado no bloquee el consumo.
- Cada permiso de IAM acotado al recurso que lo necesita: ninguna política con comodín.

