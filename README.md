![http://www.ore-hybam.org/](http://www.ore-hybam.org/var/ezwebin_site/storage/images/design/ore-hybam-the-environmental-research-observatory-on-the-rivers-of-the-amazon-basin/5007-93-eng-US/The-Environmental-Research-Observatory-on-the-Rivers-of-the-Amazon-Orinoco-and-Congo-Basins.png)

This is the experimental software laboratory for the HyBAm Observation Service. Its main purpose is to standardize development across multiple platforms and make our software readily available for public and scientific use.

## HOW TO USE IT?
First you need to install Docker Engine Community:

[WINDOWS](https://docs.docker.com/docker-for-windows/install/) | [LINUX](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
--- | ---

If everything went smoothly, then you should see something like this:
```sh
$ docker --version
Docker version 19.03.1
```
And now you can pull our container image from [Dockerhub](https://hub.docker.com/r/hybam/hybam-dev):
```sh
$ docker pull hybam/hybam-dev:beta
```
After the container image finished downloading, you can use it to create your own container, like this:
```sh
$ docker run -it --name my-container-name hybam/hybam-dev:beta
```
And thats it, now you should see an open `bash` awaiting for your command line:
```console
root@ce6847a57dca:/# ls
bin   dev  git-repositories  lab-data  lib64  mnt  proc  run   srv  tmp  var
boot  etc  home              lib       media  opt  root  sbin  sys  usr
```
This container has the following libs installed:

software | version |
--- | --- |
GDAL | 3.1.0 |
OpenJDK 8 | 1.8.0_212 |
ESA SNAP | 7.0 |
snappy | 7.0.0 |
Python | 3.6.9 |
matplotlib | 3.1.2 |
PyPDF2 | 1.26.0 |
scipy | 1.4.0 |
scikit-learn | 0.22 |
pysptools | 0.15.0 |


