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
