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

git clean [-df]
remove recursivamente os untracked files

Working directory -> Stage -> Repository
untracked files -> tracked modified -> tracked unmodified

## Docker

- **docker pull \<image-name\>**

Downloads the image


- **docker run \[commands\] \<image-name\>**

Creates a container from specified image


- **docker run -p \<host-port\>:\<exposed-container-port\> \<image-name\>**

Specifies the running port

- **docker exec -it \[container-id\] bash**

enter a running container

- **docker logs \<container\>**

read the logs from a docker

- **docker cp \<container\>:\<file\> \<destination\>**

copies a file from a container


### other parameters

-d: Detached

-it (-i -t): prints outputs

--name \<name\>: specifies a name to the container

## Mongo

mongoexport --host \<host\> --port \<port\> --db \<db name\> --collection \<collection name\> --out \<file name\>
  
mongoimport --host \<host\> --port \<port\> --db \<db name\> --collection \<collection name\> --file \<file name\>

