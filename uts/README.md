ianmujahid@Rianesians:~$ $sudo docker -v

Command 'docker' not found, but can be installed with:

sudo snap install docker     # version 18.09.9, or
sudo apt  install docker.io  # version 19.03.2-0ubuntu1

See 'snap info docker' for additional versions.

rianmujahid@Rianesians:~$ sudo snap install docker     # version 18.09.9
[sudo] password for rianmujahid: 
docker 18.09.9 from Canonical✓ installed
rianmujahid@Rianesians:~$ $sudo docker -v
Docker version 18.09.9, build 1752eb3
rianmujahid@Rianesians:~$ mkdir utstc
rianmujahid@Rianesians:~$ cd utstc
rianmujahid@Rianesians:~/utstc$ #imagebase
rianmujahid@Rianesians:~/utstc$ FROM nginx:alpine
FROM: command not found
rianmujahid@Rianesians:~/utstc$ #imagebase 
rianmujahid@Rianesians:~/utstc$ #image baseFROM nginx:alpine#copy aplication fileCOPY html /usr/share/nginx/htmlLangkah-5:
rianmujahid@Rianesians:~/utstc$ mkdir html
rianmujahid@Rianesians:~/utstc$ cd utstc
bash: cd: utstc: No such file or directory
rianmujahid@Rianesians:~/utstc$ cd..
cd..: command not found
rianmujahid@Rianesians:~/utstc$ cd
rianmujahid@Rianesians:~$ touch utstc/Dockerfile
touch: cannot touch 'utstc/Dockerfile': No such file or directory
rianmujahid@Rianesians:~$ touch utstc/Dockerfile.txt
touch: cannot touch 'utstc/Dockerfile.txt': No such file or directory
rianmujahid@Rianesians:~$ mkdir utstc
rianmujahid@Rianesians:~$ cd utstc
rianmujahid@Rianesians:~/utstc$ touch dockerfile
rianmujahid@Rianesians:~/utstc$ cd dockerfile
bash: cd: dockerfile: Not a directory
rianmujahid@Rianesians:~/utstc$ mkdir html
rianmujahid@Rianesians:~/utstc$ cd html
rianmujahid@Rianesians:~/utstc/html$ touch index.html
rianmujahid@Rianesians:~/utstc/html$ cd
rianmujahid@Rianesians:~$ cd utstc
rianmujahid@Rianesians:~/utstc$ cd Dockerfile
bash: cd: Dockerfile: No such file or directory
rianmujahid@Rianesians:~/utstc$ $sudo docker build -t aplication:versi-1
"docker build" requires exactly 1 argument.
See 'docker build --help'.

Usage:  docker build [OPTIONS] PATH | URL | -

Build an image from a Dockerfile
rianmujahid@Rianesians:~/utstc$ sudo docker images
[sudo] password for rianmujahid: 
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
rianmujahid@Rianesians:~/utstc$ sudo docker run -d -p 80:80 aplication:versi-1
Unable to find image 'aplication:versi-1' locally
docker: Error response from daemon: Get https://registry-1.docker.io/v2/: net/http: request canceled while waiting for connection (Client.Timeout exceeded while awaiting headers).
See 'docker run --help'.
rianmujahid@Rianesians:~/utstc$ $sudo docker ps
Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get http://%2Fvar%2Frun%2Fdocker.sock/v1.39/containers/json: dial unix /var/run/docker.sock: connect: permission denied
rianmujahid@Rianesians:~/utstc$ $curl -XGET localhost
-XGET: command not found
rianmujahid@Rianesians:~/utstc$ $sudo docker build -t aplication:versi-1
"docker build" requires exactly 1 argument.
See 'docker build --help'.

Usage:  docker build [OPTIONS] PATH | URL | -

Build an image from a Dockerfile
rianmujahid@Rianesians:~/utstc$ 

