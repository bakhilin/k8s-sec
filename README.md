# k8s + docker manual for P3234


## Installation
``` Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```


```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
## Commands for our seminar
### Docker
```
docker pull ubuntu
```
```
docker ps -a 
```
```
docker run -it -d ubuntu # if you want to close container, write 'exit'
```
```
docker stop container_id
```

## Список терминов, которые употребялись на докладе и их определения.
<b>Контейнер<b> - Контейнер - это стандартная программная единица, которая упаковывает код и все его зависимости, чтобы приложение быстро и надежно запускалось из одной вычислительной среды в другую.


## License

[MIT](https://choosealicense.com/licenses/mit/)
