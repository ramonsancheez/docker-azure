# docker-azure

Para realizar la práctica tenemos que crear una máquina virtual en Microsoft AZURE:
<img width="1070" alt="image" src="https://user-images.githubusercontent.com/91556453/169309632-163b0ba9-21a3-4ece-8590-e65ff0bd923c.png">

Configuramos todos los datos básicos de la máquina, y, le damos a **revisar y crear**. Seguídamente, descargamos la clave privada y creamos el recurso:
<img width="338" alt="image" src="https://user-images.githubusercontent.com/91556453/169310422-7372b6b5-a5fd-495e-bed9-e7bfb8900b28.png">

Con la siguiente imagen, corroboramos que la clave se ha creado sin problemas:
<img width="595" alt="image" src="https://user-images.githubusercontent.com/91556453/169310645-2e42b83f-71ed-4bbb-ab07-a2ad0d287e39.png">

Mediante el siguiente comando, nos conectamos a la máquina.
```bash
ssh -i ruta_clave_privada nombre_usuario@ip_maquina
```

Una vez dento la máquina, actualizaremos todos los paquetes:
```bash
sudo apt-get update
```

El siguiente paso, es instalar git para clonar el reposiotrio que deseamos dockerizar:
```bash
sudo apt-get install git
```

Y ahora, instalamos docker:
```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
```

El siguiente comando, lo utilizaremos para ejecutar el contenedor:
```bash
sudo docker run nombre_imagen
```
