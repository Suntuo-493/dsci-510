Deploy mnist application in docker
====

Create the model
------
This model is python application with Concolutional Neural Networks.<br>
After training for 20000 times. It will has about 99.5% accuracy.<br>
The Model will be saved in a file folder called Save.<br>

Set the docker
------
In this project the application will be deployed in the docker container.<br>
<br>
First, put requirements,Dockerfile and app.py in the same filefolder.<br>
And use the following command:<br>
```Bash
sudo docker build -t mnist-app:latest .
```
<br>
Second,run the Docker container<br>
We can run our docker container for testing<br>

```Bash
sudo docker run -d -p 9042:9042 mnist-app
```
<br>
Finally,Check the container by:<br>