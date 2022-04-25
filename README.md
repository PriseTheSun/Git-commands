# Comandos Git
## 1 - Iniciando um Repositório
Todo repositørio Git armazena as informações dentro de uma pasta oculta chamada “/.git”. Para que os arquivos de uma pasta possam ser versionados pelo Git, é preciso iniciar o repositório. Basta executar o comando abaixo:

#### $git init


## 2 - Apagando um repositório
Há momentos em que não queremos apagar nossos arquivos, mas queremos remover as informações sobre aquele repositório criado com o $ git init (talvez criar um repositório novo com os mesmos arquivos). Para isso não usamos o Git. Lembre-se que um repositório Git armazena as informações dentro de uma pasta oculta chamada /.git. Então basta apagar esta pasta oculta que o seu atual diretório deixará de ser um repositório.

#### $ rm -rf .git

## 3 -Listando Arquivos Modificados
Esse comando indica o estado do seu repositório. Em outras palavras, ele vai listar todos os arquivos que foram modificados desde o seu último commit.

#### $ git status


## 4 - Desfazendo Alterações
Poderíamos ter um post inteiro apenas falando sobre como desfazer alterações no Git, já que há vários cenários possíveis. Mas vamos resumir os principais:

## 4.1 - Arquivos não monitorados
Se o arquivo foi modificado mas você ainda não executou git add, um simples git checkout removerá as alterações, deixando o arquivo como ele estava no último commit. Passe o nome do arquivo a ter as alterações desfeitas ou . para desfazer as alterações em todos os arquivos modificados. Muito útil se você está apenas experimentando um código mas não quer que ele seja salvo.

#### git checkout .

Esse comando não apaga novos arquivos. Para apagar novos arquivos que ainda não foram adicionados ao Stage, execute:

#### git clean -df

## 4.2 - Removendo arquivos do Stage

Se você executou <b> git add </b> e quer desfazer, use o <b>reset.</b>

#### git reset
