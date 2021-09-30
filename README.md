# Conversao Peso (Iniciativa Kubernetes)

## Passo-a-passo do processo de montagem e execução da aplicação utilizando Docker
  1 - Criar arquivo Dockerfile dentro do diretório do projeto, contendo as instruções para criação da imagem da aplicação utilizando o Multistage Build    
  2 -  Fazer o build da imagem da aplicação:
  ```bash 
  docker image build -t brunocesar96/conversao-peso:v1 .
  ```
  3 - Rodar aplicação em um container Docker:
  ```bash 
  docker container run -d -p 5000:80 brunocesar96/conversao-peso:v1
  ```
