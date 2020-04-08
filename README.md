# Github

### Ciclo de vida dos arquivos git

Untracked = "arquivo foi criado mas nao foi visto pelo git"

unmodified = "arquivo existente no git, porém nao modificado"

modifiedd = "arquivo modificado"

staged = "pronto para ser commitado {criado uma versao dele}"



![Imagem_Ciclo_Git](https://github.com/hugoleogs/comandos_git_github/blob/master/git.png)


### Comandos do GIT

Comandos                                             |  Descrição
---------------------------------------------------- | ---------------------------------------------------------------- 
git config --global user.name "seu nome"             |  Configura seu nome
git config --global user.email "seu email"           | Configura seu email
git config --global core.editor "nome do seu editor" | Configura seu editor de texto
git config --list                                    | Lista todas as configurações do seu git
git init                                             | Inicializa o repositorio git
git status                                           | Reportar o status do repositorio no exato momento
git add "nome_do_arquivo"                            | Adiciona o arquivo ao status(staged) de ser comitado
git commit -m "uma mensagem"                         | Cria uma imagem/snapshot e o '-m' serve para colocar uma descrição
git add "nome_do_arquivo"                            | Adiciona o arquivo ao status(staged) de ser comitado 
git commit -m "uma mensagem"                         | Cria uma imagem/snapshot e o '-m' serve para colocar uma descrição 
git log                                              | Exibe: Commit, Author e Date
git log --decorate                                   | Exibe mais informações dos commit
git log --author="nome do autor"                     | Filtra pelo Autor
git log --graph                                      | Exibe de forma Grafica
git shortlog                                         | Filtra em ordem Alfabetica
git shortlog -sn                                     | Filtra com o numero de commit e nome
git show "hash"                                      | Exibe informações do que foi alterado
git diff                                             | mostra o q foi adicionado no arquivo
git diff --name-only                                 | mostra somente o arquivo modificado
git checkout 'nome_do_arquivo'                       | Retorna o arquivo para antes da edição
git reset HEAD 'nome_do_arquivo'                     | Remove o arquivo da fila do staged
git clone 'link'                                     | Clona o diretorio do github para sua maquina 
git ckeckout -b 'nome_do_branch'                     | Cria um novo branch ex: master_2
git branch                                           | Lista os branchs existentes
git ckeckout 'nome_do_branch'                        | Entra no branch selecionado
git branch -D 'nome_do_branch'                       | Apaga o branch selecionado 
git remote                                           | permite criar, ver e excluir conexões com outros repositórios
git remote -v                                        | Igual ao comando acima, mas inclui a URL de cada conexão
git push origin master                               | Usado para subir o seu commit para o seu diretorio no github
git tag -a x.x.x -m "descrição"                      | Cria uma tag
git push origin master --tags                        | Sobe a tag para o github


### Desfazendo commits                             
Comandos                                            | Descrição
--------------------------------------------------- | ---------------------------------------------------------------- 
git reset --soft "hash"                             | Retorna o comit para a versao anterior e volta para o estagio de staged
git reset --mixed "hash"                            | Retorna o comit para a versao anterior e volta para o modifiedd
git reset --hard "hash"                             | Retorna o comit para a versao anterior e ignora tudo



