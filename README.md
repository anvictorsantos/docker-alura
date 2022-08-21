## Steps to initialize this project

## Tutorial's and Stack's that helped me to understand and implemente docker with laravel

1. I used Alura Course for this project:

   1.1 If u have the project already alive in container, use this command to get him down: docker-compose down
   1.2 Now u have to enter in project root and type in terminal: docker build -t my-project/app-node:1.0 .
   1.3 After docker get your Node image, u can type in terminal the follow command to initialize the project: docker run -p 8080:3000 -d antonio/app-node
   1.4 Now u can acess trought web: http://localhost:8080/
   1.5 Command to stop all container's at same time: docker ps -aq | xargs -n 1 docker stop
   1.6 Command to kill all container's, after stop it, at same time: docker ps -aq | xargs -n 1 docker rm
   1.7 To push to repository u need to type two commands:
   1.7.1 U must need login with your account: docker login -u <docker-hub-name>
   1.7.2 This command copy and create a new tag with your docker hub name: docker tag <image-name>/app-node:1.2 <docker-hub-name>/app-node:1.2
   1.7.3 This command push to your docker repository: docker push <image-name>/app-node:1.2
