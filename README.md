
![radartona](https://github.com/guica/api_dados_radar/blob/master/media/admin-interface/logo/75125107_2420153768241552_3174633533629005824_o.png?raw=true)
# API para Dados de Radares

## Apresentação

![apresentacao](https://github.com/guica/api_dados_radar/blob/master/media/Swagger-UI.gif)

## Acesso para o Ambiente de homologação

API - http://radartona.portalretina.com/docs/

Front - http://radartona.portalretina.com/admin/

`Usuário`: admin
`Senha`: admin

## Começando

Essas instruções fornecerão uma cópia do projeto em execução na sua máquina local para fins de desenvolvimento e teste. Consulte implantação para obter notas sobre como implantar o projeto em um sistema em ambiente de produção.

### Pré-requisitos

-   Docker
-   docker-compose

Install  [Docker](https://docs.docker.com/engine/installation/)  and  [Docker compose](https://docs.docker.com/compose/install/)

### Instalando
Clone o repositório e entre no seu diretório

`git clone https://github.com/guica/api_dados_radar.git`

`cd api_dados_radar`

Crie um arquivo .env:

`touch .env`

Construa a imagem em Docker, suba o container e entre nele

`sudo docker-compose build`

`sudo docker-compose up -d`

`sudo docker-compose exec web bash`

Crie um super-usuário:

`python manage.py createsuperuser`

Entre em http://localhost:8000/admin e faça seu login. Você pode usar essa interface para navegar e explorar os dados. Depois, entre em http://localhost:8000/docs para ver a documentação da API. 

## TODO

- Melhorar Segurança
- Melhorar Escalabilidade
- HTTPS
- Throttle e logs de uso


## Contruido com

* Python 2.7
* Django 1.11.8
* Django Rest Framework
* Docker
* Docker-Compose
* Nginx

## Authors

* **Guilherme Camargo**  - [LinkedIn](https://www.linkedin.com/in/guilherme-camargo-82029b142/)

* **Paulo Henrique da Silveira** - [LinkedIn](https://www.linkedin.com/in/phsilveira/)

## License

Este projeto está licenciado sob a licença MIT - consulte o arquivo [LICENSE.md](LICENSE.md) para mais detalhes.
