# portfolioale

Projeto que mostrará meu portfolio de projetos / códigos usados para mostrar minhas habilidades no mundo do desenvolvimento de software.

Aqui voce encontrará projetos envolvendo as seguintes linguagem / frameworks / banco de dados / cloud

- java
- python
- c++
- javascript

- angular

- mysql

- aws
- azure
- google

Steps to create this project

1. Create a new repository on GitHub called portfolioale
2. Create the package.json file with "npm init -y"
3. Create a new core folder for the project
4. Create the index.ts file for typescript
5. Install the nestjs https://nestjs.com/ in the project to create the backend app with the following command:
   /c/SoftwareDevelopment/portfolioale (main)  
   $ npm i -g @nestjs/cli
6. modify :

- backend package.json the proprieties to start the backend:
  "start": "nest start --entryFile backend/src/main",
  "start:dev": "nest start --watch --entryFile backend/src/main",
- backend app.service.ts adding the following:
  import { x } from '@core';

7. execute the backend with:
   npm run start:dev

8. run the browser with the url localhost:3000 to see the app.service.ts webpage

9. supabase.com - to create database
   pwd: PE2p6EDZrmnSvsGm
   create the project

10. prisma.io

Then, install the Prisma CLI as a development dependency in the project of the backend:
npm install prisma --save-dev

Finally, set up Prisma ORM with the init command of the Prisma CLI:
npx prisma init

11. edit the schema.prisma to add the bd
12. run the following command to sync the schema.prisma with the online db on prisma.io
    npx prisma migrate dev

13. open the prisma.io to import the entries of the tecnologias.csv file;

14. n8n.io project - ferramenta para criar fluxos no-code - usaremos para conectar com nossa app
    pwd: PE2p6EDZrmnSvsGm

15. create the modules db / projeto / tecnologia in the backend folder
    nest g module db
    nest g module projeto
    nest g module tecnologia

16. create the controler and the prisma/db model
    nest g co projeto --no-spec --flat
    nest pr projeto.prisma --no-spec --flat

17. execute the back end to see and access the api end point
    npm run start:dev
    access:
    localhost:300/tecnologias
    localhost:300/tecnologias/1
    localhost:300/projetos
    localhost:300/projetos/2

nest -- help ## to see the nest command parameters available

git of the course
https://github.com/portfolio-projetos-dev
