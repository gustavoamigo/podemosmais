# podemosmais

## Instalando versão local.

Instalar Docker no Ubuntu
Ref: https://docs.docker.com/installation/ubuntulinux/

    curl -sSL https://get.docker.com/ | sh
    sudo usermod -aG docker ubuntu


Instalar Docker Compose no Ubuntu
Ref: https://github.com/docker/compose/releases

    sudo sh
    curl -L https://github.com/docker/compose/releases/download/1.4.1/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
    chmod +x /usr/local/bin/docker-compose

Alterar o hosts para apontar para o podemosmais.tk, acrescentar a seguinte linha
    
    127.0.0.1 podemosmais.tk comuna.pomdemomais.tk

Copiar o `wordpress.env.template` para `wordpress.env`. Editar e apontar para o mysql local. 

Subir o ambiente
     
     docker-compose up
     
Depois, para baixar o ambiente.   

     docker-compose stop

