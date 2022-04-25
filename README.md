# Comandos Git
## 1 - Iniciando um Repositório
### Todo repositørio Git armazena as informações dentro de uma pasta oculta chamada “/.git”. Para que os arquivos de uma pasta possam 
ser versionados pelo Git, é preciso iniciar o repositório. Basta executar o comando abaixo:

#### $git init


## 2 - Apagando um repositório
### Há momentos em que não queremos apagar nossos arquivos, mas queremos remover as informações 
sobre aquele repositório criado com o $ git init (talvez criar um repositório novo com os mesmos arquivos). 
Para isso não usamos o Git. Lembre-se que um repositório Git armazena as informações dentro de uma pasta oculta chamada /.git. 
Então basta apagar esta pasta oculta que o seu atual diretório deixará de ser um repositório.

#### $ rm -rf .git

## 3 -Listando Arquivos Modificados
### Esse comando indica o estado do seu repositório. Em outras palavras, 
ele vai listar todos os arquivos que foram modificados desde o seu último commit.

#### $ git status
