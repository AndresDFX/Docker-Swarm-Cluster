<div align="justify">

<h1><u> Descripcion</u></h1>
Lorem ipsum


<u><b>Prerrequisitos:</b></u>

* Docker Engine - 20.10.8
* Docker Compose - 1.29.2
* Python - 3.10.2

<u><b>Construido con:</b></u>

* Docker Machine
* Flask - 2.0.3
* EC2 (AWS)


---
<h2><u>Docker Swarm</u></h2>

Lorem

Para instalar docker-machine ejecutamos el siguiente comando:

```bash
curl -L https://github.com/docker/machine/releases/download/v0.16.2/docker-machine-`uname -s`-`uname -m`>/usr/local/bin/docker-machine &&\  chmod +x /usr/local/bin/docker-machine
```

Lorem

```bash
docker-machine create --driver amazonec2 --amazonec2-access-key AKI******* --amazonec2-secret-key 8T93C******* aws-node
```

Lorem

```bash
docker-machine ssh xxxxxxx
docker-machine ssh aws-node
```


Para la comunicacion entre nodos (trabajadores o administradores) se deben abrir los puertos TCP (2377, 4789, 7946) y UDP (7946) por defecto en un cluster local podemos hacerlo con los siguientes comandos desde el terminal:
```bash
sudo ufw enable
sudo ufw allow 2377/tcp
sudo ufw allow 7946/tcp
sudo ufw allow 7946/udp
sudo ufw allow 4789/tcp
sudo ufw reload
```

Si el cluster se encuentra corriendo en un ambiente de tipo cloud la mejor opcion es realizar la apertura de puertos desde el dashboard o herramienta dispuesta para este proposito segun sea el proveedor.

---
<h2><u>Docker Compose</u></h2>


---
<h2><u>Docker Swarm mode</u></h2>

---
<h2><u>Ejecutar app multicontenedor</u></h2>