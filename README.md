# Avaliacoes-M7-Inteli
Avaliações do Módulo 7

Essa aplicação contém os seguintes 3 arquivos de Docker:

- Dockerfile de frontend: Esse arquivo é composto com os comandos necessários para rodar um servidor Nodejs que nos servirá a interface.
    - Utilização da imagem base do Node
    - Instalação de todos os requisitos por meio do package.json
    - Exposição da porta utilizada
    - Inicialização do script principal

- Dockerfile de backend: Esse arquivo é composto com os comandos necessários para rodar um servidor FastAPI.
    - Utilização da imagem base do Python
    - Instalação de todos os requisitos por meio do requirements.txt
    - Exposição da porta utilizada
    - Inicialização do script principal

- Arquivo docker-compose: Esse arquivo possui todos os serviços necessários nessa aplicação (frontend e backend). Em ambos, as seguintes características são definidas.
    - A imagem que será utilizada e que se encontra no DockerHub
    - A definição de restart como always, em caso de erro, o serviço é rodado novamente
    - Conexão da porta do host com a porta do container, elas foram definidas como iguais para maior facilidade.
    - Definição do nome do container

Para executar a aplicação:

```bash
docker-compose up
```
