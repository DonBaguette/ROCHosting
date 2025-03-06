<h1 align="center">
	<align: left;">
    <img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Logo.png?raw=true
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

> [!NOTE] Text for Note

| MÁQUINA | SO | ALMACENAMIENTO | CPU | RAM | IP |
| --- | --- | --- | --- | --- | --- |
| Host | Windows 11 | 3TB SSD | 16 Núcleos | 32GB | **DHCP** 192.168.1.10 |
| pfsense | FreeBSD | 25GB SSD | 2 Núcleos | 2GB | **WAN** 192.168.1.100 / **LAN** 10.0.0.1  |
| DNS | Windows Server | 10GB SSD | 2 Núcleos | 4GB | **DHCP** 10.0.0.15 |
| Docker / Web | Ubuntu Desktop | 100GB SSD | 4 Núcleos | 8GB | **STATIC** 10.0.0.11 |

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
    <img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Networks.png?raw=true
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
  <summary>📂DNS & DHCP</summary>
    <em>
        
</p>

**DNS**
- **¿Qué es?:** El DNS es un sistema que traduce nombres de dominio legibles (como google.com) en direcciones IP numéricas que los ordenadores usan para comunicarse en la red.
- **¿Por qué es necesario?:** El DNS es necesario porque facilita la navegación en Internet al traducir nombres de dominio fáciles de recordar (como google.com) en direcciones IP que los ordenadores utilizan para comunicarse. Sin DNS, tendríamos que memorizar largas secuencias de números para acceder a los sitios web.
- **¿Dónde hay información oficial?:** En el propio microsoft oficial podemos encontra información sobre ello [DNS](https://learn.microsoft.com/es-es/windows-server/networking/dns/dns-overview)
<details>
    <summary>⚙️ Pasos para instalar el DNS en Windows Server</summary>
        <em>
        
</p>

# Configuración de Servidor DNS en Windows Server

---

## 1. Requisitos

✅ Windows Server instalado y funcionando  

✅ Acceso al servidor con sesión iniciada

---

## 2. Instalación del Servicio DNS

1. Acceder a **Windows Server** e iniciar sesión.
2. Ir a **Administrar > Agregar roles y características**.
3. Seleccionar **Servidor DNS**.
4. Iniciar la instalación y esperar a que finalice.

---

## 3. Configuración Inicial del DNS

1. Ir a **Herramientas > DNS**.
2. Hacer clic derecho en el servidor y seleccionar **Agregar Zona nueva**.
3. Seleccionar **Zona nueva**.
4. Asignar un nombre a la zona.
5. Marcar la casilla: **Crear un archivo nuevo con este nombre de archivo**.
6. Finalizar la configuración de la zona.

---

## 4. Creación de un Host Nuevo (A o AAAA)

1. Dentro de la zona creada, hacer clic derecho y seleccionar **Host nuevo (A o AAAA)**.
2. Asignar un nombre al host.
3. Introducir la dirección IP correspondiente.
4. Hacer clic en **Agregar Host**.
5. Guardar y aplicar los cambios.

---

## 5. Aplicar Configuración Final

🔒 Guardar todos los cambios.  
✅ El servicio DNS quedará habilitado y funcionando.

---
<h1 align="center">
<align: left;">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Dns.png?raw=true

  <p align="center">
  </details>
    

**DHCP**
- **¿Qué es?:** El DHCP es un protocolo que asigna automáticamente direcciones IP y otros parámetros de red a los dispositivos en una red.
- **¿Por qué es necesario?:** Es necesario porque simplifica la gestión de direcciones IP, evitando la configuración manual y reduciendo errores. Además, optimiza el uso de direcciones IP y permite que los dispositivos se conecten fácilmente a la red sin que el usuario tenga que intervenir
- **¿Dónde hay información oficial?:** En el propio microsoft oficial podemos encontra información sobre ello [DHCP](https://learn.microsoft.com/es-es/windows-server/networking/technologies/dhcp/dhcp-top)
<details>
    <summary>⚙️ Pasos para instalar DHCP en pfSense</summary>
        <em>
        
</p>

# Configuración de Servicio DHCP en pfSense

---

## 1. Requisitos

✅ pfSense instalado y funcionando en una máquina virtual  

✅ Acceso a la interfaz web de pfSense  

---

## 2. Acceder a pfSense

1. Abrir la interfaz web de pfSense.
2. Iniciar sesión con las credenciales de administrador.

---

## 3. Habilitar el Servicio DHCP

1. Ir a **Services > DHCP Server**.
2. Seleccionar la interfaz **LAN**.
3. Activar la casilla:  
   ✅ **Enable DHCP Server on LAN interface**.

---

## 4. Configurar el Rango de Direcciones IP

- Definir el rango de direcciones IP.  
  **Ejemplo:** 10.0.0.11 - 10.0.0.243

---

## 5. Aplicar Configuración Final

🔒 Guardar todos los cambios.  
✅ El servicio DHCP quedará habilitado.

---

## 6. Nota Extra

📌 Normalmente, en la configuración inicial de pfSense, el asistente te pregunta si deseas habilitar DHCP. Si lo activas ahí, este proceso se realiza automáticamente.

---
<h1 align="center">
<align: left;">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Dhcp.png?raw=true
  <p align="center">
       
  </details>
    
</details>

<details>
  <summary>📂APACHE</summary>
    <em>
        
</p>

**APACHE**
- **¿Qué es?:** Apache es un servidor web de código abierto que utiliza HTML.
- **¿Por qué es necesario?:** Apache es necesario si quieres crear una web alojada por ti mismo. En lugar de utilizar servicios de hosting de pago, puedes alojar tus propias páginas web
- **¿Dónde hay información oficial?:** Puedes encontrar información oficial en la página web de Apache, donde hay de todo tipo de información sobre el tema [APACHE](https://httpd.apache.org/)
<details>
    <summary>⚙️ Pasos para instalar APACHE en Ubuntu Desktop</summary>
        <em>
        
</p>

# Instalación y configuración de Servicio Apache2

---

# 1. **Requisitos**
✅ Tener una Maquina Virtual Disponible

---

# 2. **Actualizar los paquetes del sistema**  
	- sudo apt update && sudo apt upgrade -y

---

# 3. **Instalar Apache2**  
	- sudo apt install apache2 -y

---

# 4. **Verificar servicio**
   	- sudo systemctl status apache2
   - Ir a nuestro navegador web y poner http://(IP MAQUINA)

---

# 5. **Guardar cambios y aplicar configuración**
   - Ahora guardamos los cambios y ya estaría habilitado

---

# 6. **Modificar archivo html**
   - Ahora lo que podemos hacer es modificar nuestra pagina web y hacerla como queramos, para ello vamos a ir a nuestros explorador de archivos y vamos a ir a la siguiente ruta
       - /var/www/html

---

# 7. **Pagina web modificada**
<h1 align="center">
<align: left;">
<img width="82%" src=
  <p align="center">
       
  </details>
  
</details>

<details>
  <summary>📂PFSENSE</summary>
    <em>
        
</p>

**PFSENSE**
- **¿Qué es?:** PfSense es un sistema operativo basado en FreeBSD diseñado para funcionar como un firewall. Se utiliza principalmente para poder administrar y proteger redes
- **¿Qué es FREEBSD?:** FreeBSD es un sistema operativo libre de codigo abierto, en 2005 era el sistema operativo abierto mas popular de todos, actualmente ya no se utiliza tanto pero aún continua activo
- **¿Cuáles son las principales características de Pfsense?:**
	- Firewall
 	- Soporte para VPN
  	- Control de tráfico
  	- Sistema IDS/IPS
  	- Gestión mediante interfaz web
  	- Soporte para múltiples conexiones WAN Y VLANs
- **¿Cómo se instala y configura Pfsense?:** Pfsense se instala descargando su imagen ISO desde la web oficial la cual la podemos encontrar aqui [PFSENSE](https://www.pfsense.org/download/) Hay que tener considerado lo siguiente si queremos instalarlo en un entorno virtual.
  	- Asignar suficientes recursos (Minimo: 1 CPU, 2GB RAM, 25GB DISCO)
  	- Configurar correctamente en virtualbox las interfaces de red que vamos a utilizar
  	<em>
   </p>
   
- **¿Consideras Pfsense una opción viable para empresas y redes domésticas?:** Sí, pfSense creo que es una buena opción tanto para empresas como para redes domésticas, ya que es bastante fácil de utilizar, todo se entiende bien y tiene varias herramientas que se pueden utilizar. Normalmente, los firewalls se utilizan más en empresas, pero, en definitiva, también se podrían utilizar en una red doméstica.

- **¿Qué es el port forward? Explica cómo lo has configurado:** El Port Forwarding es una técnica que permite que conexiones externas lleguen a un dispositivo dentro de una red privada

<details> 
<summary>⚙️ Pasos para instalar Pfsense y Port forward</summary>
        <em>
        
</p>

# Instalación y Configuración Básica de pfSense

---

## 1. Requisitos

✅ Máquina Virtual disponible  

✅ Al menos 2 interfaces de red  

✅ Imagen ISO de pfSense

---

## 2. Creación de la Máquina Virtual

- Crear una nueva máquina virtual
- Configurar:
    - **Primera interfaz**: Modo NAT
    - **Segunda interfaz**: Red interna

---

## 3. Instalación de pfSense

1. Iniciar la máquina virtual con la ISO de pfSense.
2. Seleccionar **Boot Multi User** y presionar **Enter**.
3. Aceptar la pantalla de bienvenida.
4. Seleccionar **Install pfSense**.
5. Elegir el idioma.
6. Seleccionar el tipo de disco (recomendado: **Auto UFS**).
7. Esperar a que termine y seleccionar **Reboot**.
8. ⚠️ **IMPORTANTE**: Retirar la ISO antes de reiniciar.

---

## 4. Configuración Inicial de Interfaces

- Asignar interfaces:
    - **WAN** → Conexión a Internet (NAT)
    - **LAN** → Red Interna

---

## 5. Configuración de Port Forwarding

1. Ir a **Firewall > NAT**.
2. Seleccionar la pestaña **Port Forward**.
3. Hacer clic en **ADD**.
4. Configurar los siguientes campos:

    | Campo                    | Valor                     |
    |---------------------|-------------------|
    | Interface                | WAN                       |
    | Protocol                  | TCP/UDP                |
    | Destination Port Range | **From:** HTTP (80) <br> **To:** (80 o el puerto que quieras) |
    | Redirect Target IP     | 10.0.0.11             |
    | Redirect Target Port  | HTTP (80)           |

5. Guardar y aplicar cambios.

---

## 6. Creación de Reglas de Firewall

1. Ir a **Firewall > Rules > WAN**.
2. Agregar una nueva regla.
3. Configurar:

    | Campo              | Valor              |
    |------------------|----------------|
    | Action                | Pass                |
    | Protocol              | TCP o UDP    |
    | Source                | Any                 |
    | Destination        | WAN Address y puerto |
    | Description        | (Lo que quieras)  |

4. Guardar y aplicar cambios.

---

## 7. Aplicar Configuración Final

🔒 Guardar todos los cambios para que pfSense quede funcionando correctamente.

---


<h1 align="center">
<align: left;">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Rules.png?raw=true
<p align="center">
	
<h1 align="center">
<align: left;">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Port%20Forward.png?raw=true
<p align="center">
       
  </details>

  </details>

  <details>
  <summary>📂PORTFORWARD / SSH</summary>
    <em>
        
</p>

- **¿Qué es?:** El port forwarding es una técnica que sirve para permitir el tráfico externo que llegue a un dispositivo específico dentro de una red local. Normalmente se utiliza en redes empresariales cuando se necesita acceder a servicios como servidores web, cámaras, etc
- **¿Por qué es necesario?:** Es necesario para permitir el acceso remoto a servidores dentro de una red privada, publicar servicios internos (servidores web, servidores de juegos, etc.) hacia Internet y facilitar la administración remota
- **¿Cuáles son las principales características de Port Forward?:**
	- Redirección de puertos específicos a dispositivos internos
   	- Permite mantener la seguridad controlando qué puertos se exponen
   	- Permite el acceso remoto a servicios internos desde cualquier parte del mundo
   	- Muy utilizado en servidores de videojuegos y servidores web
     
<details> 
<summary>⚙️ Pasos para el configurar Port Forward y SSH</summary>
        <em>
        
</p>

# Configuración Port Forward 

---

## 1. Requisitos

✅ Tener Pfsense instalado

✅ Tener acceso a la Interfaz Web 

✅ Tener otra máquina en la misma red

---

## 2. Acceder a la Interfaz Web

1. Primero vamos a ir a otra máquina que tengamos en la red interna    
2. Para poder saber cuál es nuestra IP es tan fácil como ir al FireWall y la IP es la de la red LAN  

<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Pfsense.png?raw=true />
</p>

3. Ahora para acceder a la interfaz Web del FireWall nos vamos a nuestro navegador y ponemos la IP LAN del FireWall, en mi caso la 10.0.0.1  
4. Nos va a pedir un usuario y contraseña, la default es **USUARIO** `Admin` **CONTRASEÑA** `pfsense`
5. Ahora ya estamos dentro y nos debería de aparecer un menú como este:
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Entrada.png?raw=true />
</p>

---

## 3. Crear regla de entrada

1. Para crear la regla de entrada vamos a ir a **FireWall > NAT > Port Forward** y añadir nueva regla
2. Las opciones que vamos a tener en cuenta van a ser las siguientes:

| Campo              | Valor              |
|--------------------|--------------------|
| Interfaz	     | WAN		  |
| Address family     | IPv4		  |
| Protocol	     | TCP		  |
| Destination	     | Wan Address 	  |
| Destination Port   | HTTP (80)	  |
| Redirect target IP | Address or Alias - 10.0.0.11 |
| Redirect target port | HTTP (80)	  |
| Description	     | Regla NAT en WAN	|

3. Ahora al guardar los cambios deberíamos ver algo como esto
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Natport.png?raw=true />
</p>

---

## 4. Crear Regla WAN

1. Para crear una regla en WAN vamos a ir a **FireWall > Rules > WAN** y añadir nueva regla
2. Las opciones que vamos a tener en cuenta van a ser las siguientes:

| Campo              | Valor              |
|--------------------|--------------------|
| Interfaz	     | WAN		  |
| Address family     | IPv4		  |
| Protocol	     | TCP		  |
| Source 	     | Any		  |
| Destination	     | Address or Alias - 10.0.0.11 |
| Destination Port Range | From HTTP (80) to HTTP (80) |
| Description	     | NAT Permitir trafico WAN -> LAN |
3. Ahora al guardar los cambios y deberíamos ver algo como esto
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Wanport.png?raw=true />
</p>

---

## 5. Comprobación

1. Ahora, cuando ya hemos realizado los pasos anteriores vamos a mirar si podemos ver nuestro sitio web a través del FireWall.
2. La IP que tenemos que poner en el navegador de la máquina host para poder acceder a al web es la WAN del Pfsense en este caso la mía es (192.168.1.100)
3. Como se puede ver, aqui tenemos la página web hosteada en una máquina dentro de la red interna
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Portweb.png?raw=true />
</p>

---

# Acceso al servicio SSH

---

## 1. Requisitos

✅ Tener Pfsense instalado

✅ Tener acceso a la Interfaz Web 

✅ Tener otra máquina en la misma red

---

## 2. Activación SSH

1. En esta ocasión vamos a activar el acceso al servicio SSH y así poder conectarme desde una maquina fuera de la red a una que este dentro de la red interna (WAN > LAN)
2. Vamos a ir al FireWall y vamos a crear una regla en **FireWall > NAT > Port Forward** y añadir nueva regla
3. Las opciones que vamos a tener en cuenta van a ser las siguientes:
   
| Campo              | Valor              |
|--------------------|--------------------|
| Interfaz	     | WAN		  |
| Address family     | IPv4		  |
| Protocol	     | TCP		  |
| Destination	     | Wan Address 	  |
| Destination Port   | SSH (22)	  	  |
| Redirect target IP | Address or Alias - 10.0.0.11 |
| Redirect target port | SSH (22)	  |
| Description	     | Regla NAT en WAN para SSH en DMZ	|

4. Ahora al guardar los cambios y deberíamos ver algo como esto
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Sshnat.png?raw=true />
</p>

---

## 3. Instalar OpenSSH

1. Para poder utilizar el SSH tenemos que instalarlo en la máquina donde nos queremos conectar, en este caso un Ubuntu Desktop, normalmente los windows ya lo traen instalado por defecto.
2. Para instalarlo en Ubuntu tenemos que ir a la consola y poner el siguiente comando:
`sudo apt install openssh-server`
3. Ahora que lo tenemos instalado, vamos a desactivar el FireWall, para que nos permite la conexión, para ello vamos a utilizar el siguiente comando:
`sudo ufw disable`
4. Ahora ya tenemos todo preparado

---

## 4. Comprobación

1. Ahora para comprobar que funciona vamos a ir a nuestra máquina host (WAN) y en la consola vamos a poner lo siguiente:
   Este es mi ejemplo `ssh -p 22 docker@192.168.1.100` en vuestro caso tendréis que poner el nombre de la máquina donde hemos instalado el SSH y luego la IP WAN del FireWall
2. Si todo está bien hecho deberíais poder conectaros
<p align="left">
<img width="82%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/Sshconsola.png?raw=true />
</p>

</details>
</details>	

<details>
  <summary>📂OPENVPN </summary>
    <em>
        
</p>

# OpenVPN

---

## 1. ¿Qué es una VPN y qué ventajas ofrece?

- Una VPN es una tecnología que crea una conexión segura y cifrada entre dos o más dispositivos a través de una red pública, como internet. Esta conexión lo que hace es simular que los dispositivos están en una misma red local, proporcionando privacidad y seguridad
- Las ventajas que ofrece són las siguientes:
  	- Seguridad: Cifra la conexión entre el dispositivo y el servidor VPN
  	- Privacidad: Oculta la IP real del usuario
  	- Acceso remoto: Permite acceder a redes privadas desde cualquier lugar
  	- Protección en redes públicas: Previene ataques en redes Wi-Fi públicas al cifrar la conexión

---

## 2. ¿Qué tipos de VPN hay? Muestra un esquema de cada caso

1. **VPN de acceso remoto**
- Se trata de VPNs que te permite conectar a un usuario a una red remota de forma segura
<p align="left">
<img width="52%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/VpnAR.png?raw=true />
</p>

2. **VPN de sitio a sitio**
- Este es un tipo de VPN que conecta dos redes enteras entre sí. De esta manera, incluso si las redes están en distintas zonas geográficas, podrán estar interconectadas y funcionar como una sola.
<p align="left">
<img width="52%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/VpnSS.png?raw=true />
</p>

3. **VPN basadas en cliente**
- Estas VPN se basan en una aplicación que te instalas en el dispositivo donde quieras usarla, y desde él te conectas al servicio que tengas contratado. Son las más comunes y fáciles de utilizar.
<p align="left">
<img width="52%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/VpnBC.png?raw=true />
</p>

4. **VPN basadas en servidor**
- Es un tipo bastante más complejo, aunque con más flexibilidad y la VPN se instala directamente en un servidor al que te conectas.
<p align="left">
<img width="52%" src=https://github.com/DonBaguette/ROCHosting/blob/main/Images/VpnBS.png?raw=true />
</p>
