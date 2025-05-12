# Deploying the project on AWS EC2  

1. Clone this project in the remote VM
```
git clone https://github.com/dhruv14385/node-js-app-port-3000.git
```
2. Setup the following environment variables - `(.env)` file
```
DOMAIN= ""
PORT=3000
STATIC_DIR="./client"

PUBLISHABLE_KEY=""
SECRET_KEY=""
```

3. Initialise and start the project
```
npm install
npm run start
```

# Deploying the project on Docker  
•	Install Docker  
```
sudo apt install docker.io
```
•	Change your directory to ‘node-todo-cicd’ and build image from Dockerfile within that directory. This Dockerfile has base image of NodeJS. It exposes port 8000 and run the app when you will create a container from it.  
```
sudo docker build . -t todo-note-app
```
•	Create a container from the image
```
sudo docker run -d --name node-todo-app -p 8000:8000 todo-note-app
```
•	Open browser and type &lt;EC2-Public-IPv4&gt;:8000 and you should see the app running, this time on a Docker container.  



