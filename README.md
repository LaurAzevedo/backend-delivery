# Cupdelivery

Projeto de um delivery de cupcakes desenvolvido para o trabalho final do curso de Engenharia de Software.

- Backend: https://github.com/LaurAzevedo/backend-delivery

- Aplicativo: https://github.com/LaurAzevedo/cupdelivery

- Retaguarda: https://github.com/LaurAzevedo/erpcupdelivery

- Para execução é necessário criar na raiz do projeto um arquivo .env contendo a string de conexão do banco de dados e o JWTKEY, vide exemplo abaixo

DATABASE_URL=postgres://postgres:postgrespw@localhost:5432/deliverybackend
JWT_KEY=dihfiUHFoiudhfosfF1e5sf1s1f5f1EF15

- O arquivo deliverybackend.sql foi criado utilizando o Navicat, ele contem toda a estrutura do banco de dados

- Esse projeto está utilizando docker em produção, para realizar o deploy com o docker faça os seguintes passos

docker build -t backend-cupdelivery .

docker tag backend-cupdelivery laurazevedo/backend-cupdelivery:prod

docker push laurazevedo/backend-cupdelivery:prod

O caminho laurazevedo/backend-cupdelivery:prod deve ser alterado para o caminho do seu docker hub
