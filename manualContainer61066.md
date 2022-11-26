# Laboratório de Redes
## Manual de implantação do container

Servidor de Arquivos e Container Docker de um Servidor

- Python
- docker
- cedro (servidor UFS)

## Comandos para o docker no servidor cedro

O comando a seguir executa um contêiner 

```sh
docker run -d -p 61066:61066 -it --rm  --name  servidortcpjonny -v "$PWD":/var/www/servidortcp -w /var/www/servidortcp python:2 python ./serv_sock.py
```

Iniciar o contêiner

```sh
docker start servidortcpjonny
```


