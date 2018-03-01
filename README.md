## Git
git diff
mostra as alterações nos arquivos
  
git log [--stat]
mostra a lista de commits

git stash
remove todas as alterações do projeto desde o último commit

git stash list
mostra todas as alterações salvas em stash

git stash save "<some text>"
salva as alterações em stash
  
git stash drop <id>
  
git stash pop

git stash apply <id>
  
git reset [--soft] <hash commit>
remove o commit, mas mantém os arquivos. ou leva para o working dir ou para o staging, dependendo do modo
  
git reset --hard <hash commit>
remove os commits e os arquivos dele
  
git reset [arquivo1 arquivo2, ...]
remove os arquivos a serem comitados
  
git checkout
remove todas as alterações

Working directory -> Stage -> Repository

## Docker

- **docker pull \<image-name\>**

Downloads the image


- **docker run \[commands\] \<image-name\>**

Creates a container from specified image


- **docker run -p \<host-port\>:\<exposed-container-port\> \<image-name\>**

Specifies the running port

- **docker exec -it \[container-id\] bash**

enter a running container


### other parameters

-d: Detached

-it (-i -t): prints outputs

--name \<name\>: specifies a name to the container
