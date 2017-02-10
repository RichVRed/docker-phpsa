## PHPSA - Smart Analyzer for PHP
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/phpsa.svg)](https://hub.docker.com/r/rvannauker/phpsa/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/phpsa.svg)](https://hub.docker.com/r/rvannauker/phpsa/) [![](https://images.microbadger.com/badges/image/rvannauker/phpsa:latest.svg)](https://microbadger.com/images/rvannauker/phpsa:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-phpsa.svg)](https://github.com/RichVRed/docker-phpsa) [![license](https://img.shields.io/github/license/RichVRed/docker-phpsa.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run phpsa

### Installation / Usage
1. Install the rvannauker/phpsa container:
```bash
docker pull rvannauker/phpsa
```
2. Run phpsa through the phpsa container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="phpsa" "rvannauker/phpsa" check {destination}
```

### Download the source:
To run, test and develop the PHPSA Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-phpsa.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/phpsa" --file phpsa.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/phpsa --help
```