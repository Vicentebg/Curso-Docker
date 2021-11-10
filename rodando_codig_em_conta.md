## Rodando um código em node pelo container do docker
`docker run -p -d 8080:3000 -v "C:\Users\Vicente\Desktop\volume-exemplo:/var/www" -w "/var/www" node npm start`
- Melhorando o comando de cima: `docker run -d -p 8080:3000 -v "$(pwd):/var/www" -w "/var/www" node npm start`
- Obs: A flag pwd mostra o caminho do diretório em que você está.
  Exemplo: `docker run -v "[CAMINHO_VOLUME_LOCAL:]CAMINHO_VOLUME_CONTAINER" NOME_DA_IMAGEM`


docker build -f Dockerfile - cria uma imagem a partir de um Dockerfile.
docker build -f CAMINHO_DOCKERFILE/Dockerfile -t NOME_USUARIO/NOME_IMAGEM - constrói e nomeia uma imagem não-oficial informando o caminho para o Dockerfile.
docker login - inicia o processo de login no Docker Hub.
docker push NOME_USUARIO/NOME_IMAGEM - envia a imagem criada para o Docker Hub.
docker pull NOME_USUARIO/NOME_IMAGEM - baixa a imagem desejada do Docker Hub.
