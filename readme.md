# Description
This is the main repository of the project.
# Installation
## Dependencies
- [Docker](https://docs.docker.com/get-docker/)
- [Docker compose](https://docs.docker.com/compose/install/linux/)
- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
## HTTP support
```bash
git clone https://github.com/Dilydigre/ai-face-generator.git  	# clone the repos
cd ai-face-generator										  	# move to the folder
sudo docker compose -f docker-compose_http.yml up				# start app
# note : will take time at the first start
```
## HTTPS support
**You need to generate valid Letsencrypt certificates, the service will be no longer be available in http**
- Put your certificates in `./certbot-certs/conf/`
- Install in ./ :
```bash
git clone https://github.com/Dilydigre/ai-face-generator.git  	# clone the repos
cd ai-face-generator										  	# move to the folder
sudo docker compose up											# start app
# note : will take time at the first start
```
Once all docker have started, get the IP address using docker ps and docker inspect.