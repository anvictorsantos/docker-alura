## Steps to initialize this project

## Tutorial's and Stack's that helped me to understand and implemente docker with laravel

1. I used Alura Course for this project:

   1.1 If u have the project already alive in container, use this command to get him down: docker-compose down
   1.2 Now u have to enter in project root and type in terminal: docker build -t my-project/app-node:1.0 .
   1.3 After docker get your Node image, u can type in terminal the follow command to initialize the project: docker run -d -p 8080:3000 antonio/app-node
   1.4 Now u can acess trought web: http://localhost:8080/
