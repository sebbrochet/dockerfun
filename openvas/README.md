This Dockerfile build an [openvas](http://www.openvas.org/) image based on Centos:latest

* Build image locally
```docker build -t sebbrochet/openvas .```

* Configure openvas and update data
```docker run -it --name openvas -p 9392:9392 sebbrochet/openvas openvas-setup```

* Start previously created openvas container
```docker start openvas```

* Open browser with http://<hostIP>:9392
