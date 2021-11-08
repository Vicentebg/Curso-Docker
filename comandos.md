#### Caso não queira fazer os testes em sua máquina existe este site para "treinar" os comandos
`https://labs.play-with-docker.com/`

## Comandos

- **Para baixar/criar um container** - `docker run "iso"`
	
	Exemplo: `docker run ubuntu`

- **Para listar containers ativos** - `docker ps`

- **Para listar containers baixados e que não estão ativos** - `docker ps -a`
 ![image](https://user-images.githubusercontent.com/19577547/140802090-216dfe0a-619d-4efc-b1c1-f652e603d587.png)


- **Atrelar terminal do S.O com o do docker** - `docker run -it ubuntu`

- **Para iniciar um container** - `docker start "CONTAINER ID"`

	Exemplo: `docker start 05eeeed5e5a6`

- **Para parar um container** - `docker stop "CONTAINER ID"`

	Exemplo: `docker stop 05eeeed5e5a6`

- **Para iniciar um container e já atrelhar um terminal** - `docker start -a -i "CONTAINER ID"`

	Exemplo: `docker start -a -i a69`

- **Para buscar ajuda sobre como iniciar um container** - `docker start --help`

- **Para remover containers** - `docker rm "CONTAINER ID"`
	
	Exemplo: docker rm 1b4

- **Para remover containers:** `docker rm "CONTAINER ID"`
	
	Exemplo: `docker rm 1b4`

- **Para remover containers inativos** - `docker container prune`

- **Para visualizar as imagens do docker** - `docker images`

- **Para remover imagens do docker** - `docker rmi "REPOSITORY"`
 ![image](https://user-images.githubusercontent.com/19577547/140802187-8a94686f-e17d-4f32-bfe2-6186548630f7.png)

	
	Exemplo: `docker rmi hello-world`

- **Pare instalar uma imagem especifica (baixa várias camadas)** - `docker run ubuntu:14.04`

## WEB
#### Iremos hospedar um site estático
- **Baixando imagens não oficiais(feitos por outra pessoa)** - `docker run dockersamples/static-site`

	*Obs: Está imagem é para hospedar uma página html estática*

- **Rodando este container** - `docker run -d dockersamples/static-site`

	*Obs: A flag -d serve para rodar este comando "fora"do terminal, o docker vai rodar ele, não travando o próprio*
	
- **Para linkar uma porta do container para sua máquina** - `docker run dockersamples/static-site "CONTAINER ID"`	
![image](https://user-images.githubusercontent.com/19577547/140806834-539a8ea2-71b4-4c56-8c58-a574da421c24.png)

	*Obs: A flag -P faz com que o docker atribua as portas aleatorias que ele vai escolher para o mundo externo(máquina) para poder falar com o container.*

- **Para ver qual porta o container está utilizando** - `docker port "CONTAINER ID"`

	![image](https://user-images.githubusercontent.com/19577547/140807169-48a380a9-ca08-4d88-ab07-8bc4baefc8ba.png)
