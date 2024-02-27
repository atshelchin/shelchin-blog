+++
title = "How To Install Docker on Ubuntu 22.04"
date = 2024-02-27T20:49:59+08:00
draft = false
+++

```sh
sudo apt update
```

```shell
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```

```shell
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

```shell
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

```shell
sudo apt update
```

```shell
sudo apt install docker-ce
```

```shell
sudo systemctl status docker
```
