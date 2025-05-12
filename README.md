### Deploying the project on AWS

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

