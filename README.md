<h1>Comandos Git</h1>

<h3>1 - Iniciando um Repositório</h3>
Todo repositørio Git armazena as informações dentro de uma pasta oculta chamada “/.git”. Para que os arquivos de uma pasta possam 
ser versionados pelo Git, é preciso iniciar o repositório. Basta executar o comando abaixo:

<h4>$git init</h4>


<h3>2 - Apagando um repositório</h3>
Há momentos em que não queremos apagar nossos arquivos, mas queremos remover as informações 
sobre aquele repositório criado com o $ git init (talvez criar um repositório novo com os mesmos arquivos). 
Para isso não usamos o Git. Lembre-se que um repositório Git armazena as informações dentro de uma pasta oculta chamada /.git. 
Então basta apagar esta pasta oculta que o seu atual diretório deixará de ser um repositório.

<h4>$ rm -rf .git</h4>

<h3>3 -Listando Arquivos Modificados</h3>
Esse comando indica o estado do seu repositório. Em outras palavras, 
ele vai listar todos os arquivos que foram modificados desde o seu último commit.

<h4>$ git status</h4>
