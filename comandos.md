- **Para baixar/criar um container** - `docker run "iso"`
	
	Exemplo: `docker run ubuntu`

- **Para listar containers ativos** - `docker ps`

- **Para listar containers baixados e que não estão ativos** - `docker ps -a`

- **Atrelar terminal do S.O com o do docker** - `docker run -it ubuntu`

- **Para iniciar um container** - `docker start "CONTAINER ID"`

	Exemplo: `docker start 05eeeed5e5a6`

- **Para parar um container** - `docker stop "CONTAINER ID"`

	Exemplo: `docker stop 05eeeed5e5a6`

- **Para iniciar um container e já atrelhar um terminal** - `docker start -a -i "CONTAINER ID"`

	Exemplo: `docker start -a -i a69`

- **Para buscar ajuda sobre como iniciar um container** - `docker start --help`
