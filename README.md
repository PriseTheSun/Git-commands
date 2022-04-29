# Comandos Git 
## 1 - Iniciando um Repositório
Todo repositørio Git armazena as informações dentro de uma pasta oculta chamada “/.git”. Para que os arquivos de uma pasta possam ser versionados pelo Git, é preciso iniciar o repositório. Basta executar o comando abaixo:

####  :point_right: git init


## 2 - Apagando um repositório
Há momentos em que não queremos apagar nossos arquivos, mas queremos remover as informações sobre aquele repositório criado com o $ git init (talvez criar um repositório novo com os mesmos arquivos). Para isso não usamos o Git. Lembre-se que um repositório Git armazena as informações dentro de uma pasta oculta chamada /.git. Então basta apagar esta pasta oculta que o seu atual diretório deixará de ser um repositório.

####  :point_right: rm -rf .git

## 3 -Listando Arquivos Modificados
Esse comando indica o estado do seu repositório. Em outras palavras, ele vai listar todos os arquivos que foram modificados desde o seu último commit.

####  :point_right: git status


## 4 - Desfazendo Alterações
Poderíamos ter um post inteiro apenas falando sobre como desfazer alterações no Git, já que há vários cenários possíveis. Mas vamos resumir os principais:

## 4.1 - Arquivos não monitorados
Se o arquivo foi modificado mas você ainda não executou git add, um simples git checkout removerá as alterações, deixando o arquivo como ele estava no último commit. Passe o nome do arquivo a ter as alterações desfeitas ou . para desfazer as alterações em todos os arquivos modificados. Muito útil se você está apenas experimentando um código mas não quer que ele seja salvo.

#### :point_right: git checkout .

Esse comando não apaga novos arquivos. Para apagar novos arquivos que ainda não foram adicionados ao Stage, execute:

#### :point_right: git clean -df

## 4.2 - Removendo arquivos do Stage
Se você executou :point_right: git add  e quer desfazer, use o  :point_right: reset.

#### :point_right: git reset

Para desfazer as modificações, após o reset  use o :point_right: checkout  ou :point_right: clean  mostrados anteriormente.

## 4.3 - Desfazendo o último commit
Caso você tenha feito alterações e já tenha chegado a realizar um commit, para desfazer é necessário usar o :point_right: revert.

#### :point_right: git revert HEAD

Será criado um novo commit indicando que o último commit foi desfeito. Esse comando apaga novos arquivos.

## 5 - Renomear Commit
Escreveu algo errado no último commit? Esse comando te permite renomear a mensagem do último commit feito:

#### :point_right: git commit --amend

## 6 - Branches
Sempre é bom não trabalhar apenas na main para evitar problemas e ter um projeto mais flexível.

## 6.1 - Listando Branches
Esse comando lista todas as branches presentes no repositório do seu computador.

#### :point_right: git branch
Caso você queira que ele liste também as branches que estão no repositório remoto, adicione :point_right: -a:

#### :point_right: git branch -a

## 6.2 - Indo para outra branch
Para mudar para uma outra branch basta usar o comando :point_right: checkout, passando o nome da branch.

#### git checkout minha-branch
Se você adicionar :point_right: -b, uma nova branch será criada.

#### :point_right: git checkout -b minha-nova-branch

