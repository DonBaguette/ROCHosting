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
    - **Procesador:** 2 Núcleo 
    - **Memoria RAM:** 2GB
    - **Almacenamiento:** 25GB
    - **Conexion internet:** Interfaz1 Wan (Red NAT) / Interfaz2 Lan (Red Interna)
  - **Software**
    - **Sistema Operativo:** Pfsense

**Máquina para DNS**
  - **Hardware**
    - **Procesador:** 2 Núcleo 
    - **Memoria RAM:** 4GB
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
        
</p>

- **Administrador de Red:** Configurar pfSense, DHCP y DNS *(Guillem)*
- **Desarrollador Backend:** Desarrollar la gestión de contenedores y copias de seguridad *(Guillem)*
- **Desarrollador Página web:** Crear la interfaz web para gestión y monitoreo *(Guillem)*
- **Administrador de Infraestructura:** Gestionar máquinas virtuales y rendimiento *(Guillem)*

## 📄Diagrama de la Red

<p align="center">
    <em>
        
</p>

<h1 align="center">
	<align: left;">
    <img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Diagrama%20Red.png?raw=true
  <p align="center">

  ## 📈Diagrama de Gantt (En proceso)

<p align="center">
    <em>
        
</p>

- **Semana** **: Configuración de máquinas virtuales y pfSense.
- **Semana** **: Instalación de Docker y desarrollo de la interfaz web.
- **Semana** **: Implementación de copias de seguridad y monitoreo.
- **Semana** **: Pruebas y ajustes finales.

## 📁Guías de uso 

<p align="center">
    <em>
        
</p>



<details>
  <summary><strong>📂DNS & DHCP<strong></summary>

**DNS**
- **¿Qué es?:** El DNS es un sistema que traduce nombres de dominio legibles (como google.com) en direcciones IP numéricas que los ordenadores usan para comunicarse en la red.
- **¿Por qué es necesario?:** El DNS es necesario porque facilita la navegación en Internet al traducir nombres de dominio fáciles de recordar (como google.com) en direcciones IP que los ordenadores utilizan para comunicarse. Sin DNS, tendríamos que memorizar largas secuencias de números para acceder a los sitios web.
- **¿Dónde hay información oficial?:** En el propio microsoft oficial podemos encontra información sobre ello [DNS](https://learn.microsoft.com/es-es/windows-server/networking/dns/dns-overview)
- **Pasos a seguir:**

**DHCP**
- **¿Qué es?:** El DHCP es un protocolo que asigna automáticamente direcciones IP y otros parámetros de red a los dispositivos en una red.
- **¿Por qué es necesario?:** Es necesario porque simplifica la gestión de direcciones IP, evitando la configuración manual y reduciendo errores. Además, optimiza el uso de direcciones IP y permite que los dispositivos se conecten fácilmente a la red sin que el usuario tenga que intervenir
- **¿Dónde hay información oficial?:** En el propio microsoft oficial podemos encontra información sobre ello [DHCP](https://learn.microsoft.com/es-es/windows-server/networking/technologies/dhcp/dhcp-top)
- **Pasos a seguir:**
</details>

<details>
  <summary><strong>📂APACHE<strong></summary>




</details>





