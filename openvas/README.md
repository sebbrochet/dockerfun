This Dockerfile build an [openvas](http://www.openvas.org/) image based on Centos:latest

* Build image locally   
```docker build -t sebbrochet/openvas .```

* Launch a shell with openvas image   
```docker run -it --name openvas -p 9392:9392 sebbrochet/openvas /bin/bash```

* Using the shell, configure openvas and update data   
*openvas-setup*

* Open a browser to go to https://<DockerHostIP>:9392   

* Login with previous account credentials   

* Enjoy!   

