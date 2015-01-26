This Dockerfile build an [openvas](http://www.openvas.org/) image based on Centos:latest

* Build image locally   
```docker build -t sebbrochet/openvas .```

* Launch a shell with openvas image   
```docker run -it --name openvas -p 9392:9392 sebbrochet/openvas /bin/bash```

* Using the shell, configure openvas and update data   
*openvas-setup*   

   * Vulnerabilies definitions will be downloaded, this will take several minutes.
   * Be sure to allow outgoing rsync port access (tcp/873).
   * You will be asked if you *Allow connections from any IP*, answer Yes (it is the default).
   * An account for GSAD (Greenbone Security Assistant) admin user will  be created.   
     You have to supply corresponding user/password.

* Open a browser to go to https://<DockerHostIP>:9392   

* Login with previous account credentials   

* Enjoy!   

