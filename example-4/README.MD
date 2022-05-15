# Example-4

This example demonstrates end to end testing a microservice with Cypress.

First you must boot the microservices application:

```bash
docker-compose up --build
```

Now install dependencies for testing:

```bash
cd example-4
npm install
```

Then run headless Cypress tests:

```bash
npm test
```


Or to show the Cypress UI:

```bash
npm run test:watch
```



Example-4
Docker environment is necessary,

1. Replace the ./fileName/* to /src/fineName/* in mount path in docker-compose.yml

1. run mount on powershell
```Powershell
minikube start
$current_directory = (pwd).path
minikube mount ${current_directory}:/src
```

3. run docker-compose on git bash
```bash
eval $(minikube docker-env)
docker-compose up -d
```