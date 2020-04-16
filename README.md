## Docker Nextcloud

Here there is the .yaml file for a complete deploy of a nextcloud infrastructure based on docker. 

# Install Docker on your machine ( Centos 7.6 for me )

```curl -fsSL https://get.docker.com/ | sh```

```sudo systemctl start docker```

Make sure it starts at every server reboot:

```sudo systemctl enable docker```

# Install docker-compose  

```sudo curl -L https://github.com/docker/compose/releases/download/1.21.0/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose```

```sudo chmod +x /usr/local/bin/docker-compose```

```sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose```

```docker-compose --version```

## Let's start with docker-compose.yml

At this point, in the directory in which there is the .yml file start docker-compose:

```docker-compose up```

And the magic happaned !

PS. with ```docker-compose up -d``` the output goes in backgroud
