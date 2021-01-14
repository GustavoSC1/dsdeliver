# DS Delivery
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/GustavoSC1/dsdeliver/blob/main/LICENSE) 

# Sobre o projeto

https://dsdeliver-gustavo.netlify.app

DS Delivery é uma aplicação full stack web e mobile construída durante a 2ª edição da **Semana DevSuperior** (#sds2), evento organizado pela [DevSuperior](https://devsuperior.com "Site da DevSuperior").

A aplicação consiste em um serviço de delivery, onde os pedidos são feitos no app web, e depois são listados no app mobile. No app web é possível que o cliente escolha os produtos e a sua localização, já no app mobile o dono do restaurante consegue ver a lista de pedidos, os detalhes de cada um e a localização do cliente. 

## Layout mobile
![Mobile 1](https://ik.imagekit.io/gustavosc/dsdelivery/iPhone_8_Plus_-_HOME_pBisZoF9E.jpg) ![Mobile 2](https://ik.imagekit.io/gustavosc/tr:w-413,h-736,cm-extract,x-0,y-0/dsdelivery/iPhone_8_Plus_-_PEDIDOS_I5ubBTpi3.jpg)

![Mobile 3](https://ik.imagekit.io/gustavosc/dsdelivery/iPhone_8_Plus_-_DETALHES_RxUjRLFIi.jpg)

## Layout web
![Web 1](https://ik.imagekit.io/gustavosc/dsdelivery/HOME_DELIVERY_78bOsrScb.jpg)

![Web 2](https://ik.imagekit.io/gustavosc/dsdelivery/SELECIONAR_PRODUTOS_ZIoqXqSri.jpg)

## Modelo conceitual
![Modelo Conceitual](https://ik.imagekit.io/gustavosc/dsdelivery/modelo-conceitual_pBR6G0j71.png)

# Tecnologias utilizadas
## Back end
- [Java](https://www.oracle.com/java/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [Maven](https://maven.apache.org/)
## Front end
- HTML / CSS
- [JavaScript](https://www.javascript.com/)
- [TypeScript](TypeScript)
- [ReactJS](https://pt-br.reactjs.org/)
- [React Native](https://reactnative.dev/)
- [React Leaflet](https://react-leaflet.js.org/)
- [Mapbox](https://www.mapbox.com/)
- [Expo](https://expo.io/)
## Implantação em produção
- [Back end: Heroku](https://dashboard.heroku.com/)
- [Front end web: Netlify](https://www.netlify.com/)
- [Banco de dados: Postgresql](https://www.postgresql.org/)

# Como executar o projeto

## Pré-requisitos

Para executar este projeto no modo de desenvolvimento, você precisará ter um ambiente básico para executar um Aplicativo React-Native e uma Aplicação ReactJS, que pode ser encontrado [aqui](https://www.youtube.com/playlist?list=PLNuUvBZGBA8kMTSPMmmNiRm2z0gRxXxox).

Além disso, para executar o back-end em seu computador, você também precisará ter um ambiente básico. Você pode encontrar tudo que precisa para iniciar o back-end [aqui](https://www.youtube.com/playlist?list=PLNuUvBZGBA8kMTSPMmmNiRm2z0gRxXxox).

## Back end
Pré-requisitos: Java 11

Para executar este projeto, você precisará mudar o ambiente do projeto para modo de teste. Para fazer isso vá para o arquivo /src/main/resources e edite o valor de spring.profiles.active.

Deve ser assim:

spring.profiles.active=test

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dsdeliver

# entrar na pasta do projeto back end
cd backend

# executar o projeto
./mvnw spring-boot:run
```

## Front end web
Pré-requisitos: npm / yarn

Você pode utilizar o back-end funcionando em sua máquina ou o deploy dele no Heroku, para isso acesse os arquivo src/api.ts e edite o valor de API_URL.

Deve ser assim:

const API_URL = 'https://dsdeliver-gustavo.herokuapp.com';

Ou

const API_URL = 'http://localhost:8080';

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dsdeliver

# entrar na pasta do projeto front end web
cd front-web

# instalar dependências
npm install

# executar o projeto
npm start
```

## Front end mobile
Pré-requisitos: npm / yarn

Você pode utilizar o back-end funcionando em sua máquina ou o deploy dele no Heroku, para isso acesse os arquivo src/api.ts e edite o valor de API_URL.

Deve ser assim:

const API_URL = 'https://dsdeliver-gustavo.herokuapp.com';

Ou

const API_URL = 'http://localhost:8080';

Para executar o front ent mobile você também precisará baixar o aplicativo Expo em seu smartphone e utilizá-lo para ler o QR Code que vai aparecer no terminal quando terminar o start da aplicação.

```bash
# clonar repositório
git clone https://github.com/GustavoSC1/dsdeliver

# entrar na pasta do projeto front end web
cd front-mobile

# instalar dependências
npm install

# executar o projeto
npm start
```

# Autor

Gustavo da Silva Cruz

https://www.linkedin.com/in/gustavo-silva-cruz-20b128bb/
