# DOCKER
Container
############### Instalacion de Docker #####################

```
apt install -y \
    apt-transport-https \
    ca-certificates \
curl \
    gnupg-agent \
    software-properties-common	
```

--------------- APT KEY -----------------------------------

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -				
					
apt-key fingerprint 0EBFCD88
```

--------------- Repositorio -------------------------------

```
add-apt-repository \
"deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
```

---------------- update-------------------------------------

```
apt update
```

---------------- instalar docker ---------------------------

```
apt install -y docker-ce docker-ce-cli containerd.io

sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose
```

