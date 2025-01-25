## O que é Docker

O docker veio para resolver problemas de entregas relacionados a questões de diferentes sistemas operacionais em máquinas diferentes, então pode-se criar simulações de "funciona na minha máquina" para quaisquer ambientes. Assim emulando o que uma aplicação precisaria para rodar a mesma. 

## O que é um Container

O container é uma espécie de pacote onde contém nele o sistema operacional específico para aquela aplicação, as bibliotecas e os arquivos necessários.

## O que são imagens 

Elas são instruções sobre o que deve tem no container, como organizar estrutura de pastas, quais comandos utilizar, quais arquivos necessários e entre outros comandos. OBS: Para inicializar um container é preciso ter uma imagem base como referência.


## Como executar um container

Para isso execute em seu terminal:

```bash
docker container run hello-world
```

## Como criar um container

```bash
# docker - comando - subcomando - params
docker container run <image>:<tag>
```

É possível que existam comandos que tenham abreviações não necessitando de sub-comandos
OBS: Caso nenhuma tag seja passada, vem a tag latest por padrão.
Agora executando um container ubuntu

```bash
docker container run ubuntu
```

Para visualizar os containers é possível utilizando o comando:

```bash
docker container ps
```
Já para container desativos: 

```bash
docker container ps -a
```
Para subir um container já existente podemos usar a flag `start` juntamente com o   `container_id`. 

```bash
docker container start <container_id>
```
Já para pausar esse container:

```bash
docker container stop <container_id>
```

Para remover todos os containers que não estão em uso: 
OBS: Este comando vai deletar todos os container que estiverem inativos

```bash
docker container prune
```

Para remover um container desativo é necessário usar a flag `rm` e `-f`. 

```bash
docker container rm -f <container_id>
```