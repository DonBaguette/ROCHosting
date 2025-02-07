<h1 align="center">
	<align: left;">
    <img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Logo.png?raw=true
  <p align="center">
            ROCHosting<br>
            <br><br>
        </em>
        <img src="https://img.shields.io/static/v1?label=SO&message=Ubuntu&color=orange&style=for-the-badge&logo=Ubuntu" alt="Author: Ubuntu">
    </a>
    <a href="#">
        <img src="https://img.shields.io/static/v1?label=CV&message=Docker&color=blue&style=for-the-badge&logo=Docker" alt="Docker:Docker">
    </a>
    <a href="#">
        <img src="https://img.shields.io/static/v1?label=CV&message=DockerCompose&color=0067dc&style=for-the-badge&logo=Docker" alt="Languaje:DCompose">
    </a>
  <br>
    <a  href="#">
      <img  src="https://img.shields.io/static/v1?label=SWP&message=Nginx&color=209237&style=for-the-badge&logo=Nginx"  alt="Language:Nginx">
    </a>
    <a href="#">
      <img  src="https://img.shields.io/static/v1?label=SWP&message=Playit.gg&color=563d7c&style=for-the-badge&logo=Play"  alt="Language: Playit">
    </a>
    <a href="#">
        <img src="https://img.shields.io/static/v1?label=LP&message=HTML &color=E65100&style=for-the-badge&logo=HTML" alt="Language: HTML">
    </a>
    <a href="#">
		<img  src="https://img.shields.io/static/v1?label=LP&message=Python&color=yellow&style=for-the-badge&logo=Python"  alt="Language:Python ">
	</a>
    </p>
</div>

## Tabla de contenido

<p align="center">
 <a href="#Acerca de">Acerca de</a> •
 <a href="#Características">Características</a> •
 <a href="#Requerimientos del sistema">Requerimientos del sistema</a> • 
 <a href="#installation">Instalación</a> • 
 <a href="#getting-started"></a> • 
 <a href="#technologies"></a> • 
 <a href="#license"></a>
</p>

## 📌Acerca de
<div>
    <p align="center">
    <em>
         ROCHosting es una plataforma que permite desplegar, administrar y acceder a servidores de juegos utilizando Docker. Inicialmente, el proyecto está diseñado para uso personal, con la posibilidad de expandirse a un sistema multiusuario en el futuro.
	El objetivo principal es facilitar la gestión de servidores de juegos en contenedores Docker, proporcionando una interfaz web intuitiva para iniciar, detener y configurar diferentes servidores sin necesidad de abrir puertos manualmente, gracias a la integración 	con Playit.gg.
    </em>
    </p>
</div>

## 🚀Características

 <p align="center">
    <em>
    </em>
 </p>
 
- **Implementación con Docker:** *Cada servidor de juego se ejecuta en su propio contenedor para garantizar aislamiento y fácil administración*
- **Soporte para múltiples juegos:** *Comenzando con Valheim, con la posibilidad de añadir otros juegos en el futuro como Minecraft, CS:GO, Rust, entre otros..*
- **Interfaz Web:** *Permite seleccionar, iniciar y administrar los servidores de manera sencilla*
- **Escalabilidad:** *Diseñado para crecer, con la posibilidad de convertirse en un servicio multiusuario en el futuro*
- **FireWall** *Garantiza la seguridad en la red para que no puedan atacarte ni tumbar los servidores*

## 💿Especificaciones del sistema

 <p align="center">
    <em>
 </p>

**Máquina Host**
  - **Hardware**
    - **Procesador:** 16 Núcleos
    - **Memoria RAM:** 32GB
    - **Almacenamiento:** 3TB 
  - **Software**
    - **Sistema Operativo:** Windows 11

**Máquina para pfSense (FireWall y DHCP)**
  - **Hardware**
    - **Procesador:** 1 Núcleo 
    - **Memoria RAM:** 16GB / 32GB
    - **Almacenamiento:** 25GB
    - **Conexion internet:** Interfaz1 Wan (Red NAT) / Interfaz2 Lan (Red Interna)
  - **Software**
    - **Sistema Operativo:** Pfsense

**Máquina para DNS**
  - **Hardware**
    - **Procesador:** 1 Núcleo 
    - **Memoria RAM:** 1GB
    - **Almacenamiento:** 10GB
    - **Conexion internet:** Conexión Red Interna
  - **Software**
    - **Sistema Operativo:** Windows Server

**Máquina para Contenedores Docker y Web**
  - **Hardware**
    - **Procesador:** 4 Núcleos 
    - **Memoria RAM:** 8GB / 16GB
    - **Almacenamiento:** 100GB
    - **Conexion internet:** Conexión Red Interna
  - **Software**
    - **Sistema Operativo:** Ubuntu Desktop

  
  ## 📕Roles y Responsabilidades

<p align="center">
    <em>
        
    </em>
</p>

- **Administrador de Red:** Configurar pfSense, DHCP y DNS *(Guillem)*
- **Desarrollador Backend:** Desarrollar la gestión de contenedores y copias de seguridad *(Guillem)*
- **Desarrollador Página web:** Crear la interfaz web para gestión y monitoreo *(Guillem)*
- **Administrador de Infraestructura:** Gestionar máquinas virtuales y rendimiento *(Guillem)*

## 📄Diagrama de la Red

<p align="center">
    <em>
        
    </em>
</p>





