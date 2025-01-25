## O que é o DockerFile

Para criar um container é preciso de uma imagem base, para isso podemos gerenciar quais imagens queremos com base em um arquivo `dockerfile`. Onde vamos especificar passo a passo o que vamos precisar para subir nossa imagem.

Para isso, é legal seguir um conjunto de passos.

- [ ] Definir uma imagem base.
- [ ] Definir qual versão a ser utilizada (OBS: Caso não defina, ele vai pegar a versão latest)
- [ ] Criar a pasta onde vai ficar o index do projeto
- [ ] Copiar esse arquivo para dentro da imagem 
- [ ] Definir qual a porta 
- [ ] Setar variáveis de ambiente
- [ ] Definir qual pasta vai conter o projeto
- [ ] Subir e colocar no ar (pode ser feito com ngnx)


Na pasta `./practices` tem um exemplo dos passos seguidos acima. Também para entender cada comando é necessário uma leitura na documentação `https://docs.docker.com/reference/dockerfile/`. 