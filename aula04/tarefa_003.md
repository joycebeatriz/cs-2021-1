<p style="text-align: center;"><font size="5"><b>Git Exercícios</b></font></p1></p>
<DIV align="justify">

Responda as questões abaixo (exercite os comandos do git correspondentes). Lembre-se de que o “interessante” não é exatamente o conjunto de respostas, mas o processo de obtê-las e a experiência obtida com a execução dos comandos.


1. Qual o comando para obter a versão instalada do Git?
  git version 

2. Qual o efeito da execução de cada um dos comandos abaixo?
  
  a. git help
  Exibe uma lista dos comandos mais utilizados.  

  b. git help checkout
  Abre uma guia no navegador contendo o uma página com o manual referente aos comandos "git checkout".

  c. git help merge
  Abre uma guia no navegador contendo o uma página com o manual referente aos comandos "git merge".

  d. git init
  comando utilizado para criar novo repositório. 

  e. git add --all
  Digite  git add --all  no prompt da linha de comando no diretório local do projeto para adicionar os arquivos ou alterações ao repositório. 

  f. git add -u
  examina todos os arquivos já rastreados e organiza as alterações nesses arquivos se forem diferentes ou se tiverem sido removidos. Ele não adiciona nenhum arquivo novo, apenas organiza alterações em arquivos já rastreados.

  g. git config -l
  O comando git config -l lista todos as configurações do úsuario.

  h. git mv a.txt b.txt
  Comando utilizado para renomear arquivos como a.txt para b.txt 

  i. git reset --hard
  Reset os commit e descatar todas as alterações, passando a exibir o último commit 
  
  j. git log -27
  Exibe no terminal os último 27 commits. 

3. O fluxo “clássico” de interação com o Git é algo como “alterar um ou mais arquivos”, “acrescentar essas mudanças para serem contemplados no próximo commit” e, finalmente, executar um “commit”. Quais os comandos necessários para realizar os dois últimos “passos” desse fluxo?

  git add    // adicionar 
  git rm     // remover 
  git mv     // mover ou renomear um arquivo, diretório
  git commit // executar um commit 
   
4. Qual o comando deve ser executado para identificar o que foi alterado desde o último “commit”?
   git show 

5. Em um dado repositório, arquivos simplesmente copiados para lá, ou seja, _untracked_, podem ser exibidos/identificados com que comando?
  git status


6. Qual o comando para efetuar um _commit_?
  git commit ou git commit -m para adicionar uma mensagem.  

7. Qual o comando que devemos empregar para descartar mudanças ocorridas no arquivo teste.txt, por exemplo?
  git checkout 

8. O que deve ser feito para que um determinado diretório do seu repositório seja ignorado pelo Git? Faça uma busca por **.gitignore**.
  
  Deve criar um arquivo .gitignore  para que assim ele seja ignorado pelo Git.

9.  O que acontece se o seu repositório local for acidentalmente removido?
  Haverá a perda do Repositório Local. 

10. Como clonar um repositório remoto?
    git clone 

11. Em alguns cenários **git log** pode produzir extensos resultados. Se houver interesse em visualizar o histórico de um repositório, onde cada mudança é fornecida exatamente em uma única linha, qual o comando que deve ser empregado?
  git log --pretty=oneline 

12. Em qual arquivo o Git armazena informações de configuração empregadas por usuário?
  ~/.gitconfig 

13. Qual o comando para criar um repositório local?
  Criar uma nova pasta, clicar com o botão direito dentro na opção "Git bash here" e execute o comando git init. 

14. Qual o nome do diretório criado pelo Git quando se executa o comando **git init**?
  O nome será o mesmo do repositório onde foi executadom e contém também o endereço de onde encontrar. 

15. Qual o comando para adicionar todos os arquivos modificados? (Aqueles para os quais **git status** identificam como **modified**?)
    git add --all

16. O Git faz uso do valor de hash conhecido por SHA1. O que isto significa? Qual o propósito? O que é SHA1?
  O Git foi projetado com a integridade do código-fonte gerenciado como uma prioridade. O conteúdo dos arquivos, bem como os verdadeiros relacionamentos entre arquivos e diretórios, versões, tags e commits, todos esses objetos no repositório do Git são protegidos com um algoritmo de hash de criptografia seguro chamado SHA1. Isso protege o código e o histórico de alterações contra alterações acidentais e maliciosas e garante que o histórico tenha rastreabilidade total. 
  A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA). A encriptação gera conjunto de characteres identificador de 40 dígitos. É uma forma curta de representar um arquivo.  

17. Qual a palavra para indicar o último _commit_ em vez do valor de hash SHA1 correspondente?
   -abbrev-commit 

18. Quando se cria dois arquivos usando um editor de texto qualquer e, na sequência, executamos o comando **git add -u**, os dois arquivos criados passam de _untracked_ para _new file_?
    Não, o comando git add -u adiciona os arquivos editados e que são monitorados pelo git.

19. Qual o efeito da execução dos dois comandos abaixo, nesta ordem, em um dado repositório?
    **git reset --soft HEAD~1**
    **git reset --hard**

  git reset --soft HEAD~1 // removerá o último commit do branch atual, mas as alterações do arquivo permanecerão na working tree.  
  git reset --hard //  exibe apenas o último commit realizado

20.  Após o emprego de um ambiente integrado de desenvolvimento (IDE), é comum a criação de arquivos e diretórios. Qual o comando que podemos empregar para remover arquivos e diretórios _untracked_?
  git clean -f 

21.  Qual o nome do arquivo no qual podemos inserir a indicação para o Git de arquivos e diretórios a serem ignorados?
   arquivo .gitignore  

22.  Quando se cria o arquivo _MinhaClasse.class_ em um dado diretório e desejamos que arquivos com a extensão .class, como neste caso, sejam ignorados por todos os membros de uma equipe que estão contribuindo com um dado projeto, como devemos proceder?
  *.class  

23.  jQuery é uma famosa biblioteca em JavaScript. Consulte detalhes em [jQuery](http://jquery.com). O repositório correspondente encontra-se em [gitRep](https://github.com/jquery/jquery.git). Faça o clone deste repositório.


24.  No repositório **jqueryrepo**, criado no passo anterior, qual o efeito do comando
**git shortlog -sne**?
  Exibi o nome e e-mail dos participantes. 

25. No repositório **jqueryrepo**, qual o efeito de **git remote -v**?
  Exibe o endereço de acesso (url) do diretório jquery.git 
  "https://github.com/jquery/jquery.git"

26. Um repositório Git pode ser etiquetado ao longo do tempo. Ou seja, _commits_ específicos podem ser “marcados” ou “etiquetados” para facilitar referências posteriores. Para listar todas as “etiquetas” (_tags_) estabelecidas para um dado repositório, qual comando deve ser executado?
  Deve ser executado git tag para listar todas as tags   

27. Caso um dato repositório retorne muitas “marcas” ou “etiquetas” para o comando **git tag**, como retornar apenas aquelas que atendem a determinado padrão, por exemplo, iniciadas por 2.0?
  git tag -a   

28. Qual o efeito do comando **git tag -a 3.4-gold -m “minha versão ouro”**?
  Após executado vai exibir os dados da tag junto com o commit. 

29. Após executado o comando acima, qual o efeito de **git show 3.4-gold**? 
    é possível ver os dados do autor, data, hora e ação executada. 
    
    //Descrição abaixo: 

    "Author: Michał Gołębiowski-Owczarek <m.goleb@gmail.com>
Date:   Mon Jul 19 19:04:23 2021 +0200

    Manipulation: Don't remove HTML comments from scripts

    When evaluating scripts, jQuery strips out the possible wrapping HTML comment
    and a CDATA section. However, all supported browsers are already doing that
    when loading JS via appending a script tag to the DOM which is how we've been
    doing `jQuery.globalEval` since jQuery 3.0.0. jQuery logic was imperfect, e.g.
    it just stripped the `<!--` and `-->` markers, respectively at the beginning or
    the end of the script contents. However, browsers are also stripping everyth:"

    
30. O que o comando **git push origin 3.4-gold** teria como efeito?
Iria atualizar o repositório remoto com o repositório local sob a tag 3.4-gold, caso houvesse permissão para esta ação.

31. Após executar um commit, qual o efeito de **git commit --amend**?
      O git commit --amend permite adicionar alterações ao último commit, por exemplo, na situação em que você esqueceu de adicionar alguma coisa ao último commit, seja um arquivo ou uma certa alteração aos arquivos.

32. Após executar **git add x.txt**, qual o efeito de **git reset HEAD x.txt**?
  As mudanças no arquivo e adição não serão commitadas.  

33. Após alterar o conteúdo de um arquivo committed em passo anterior, qual o efeito do comando **git checkout -- a.txt**?
  Descarta as mudanças ocorridas no arquivo. 

34. Qual a diferença entre os comandos **git reset HEAD a.txt** e **git checkout -- a.txt**?
   O comando git reset HEAD x.txt retira o arquivo x.txt da staging Area, e o git checkout -- a.txt descarta as mudanças feitas no arquivo. 

35. Veja como interpretar o resultado de git diff [aqui](https://medium.com/therobinkim/how-to-read-a-git-diff-6c87a9dc47c5). Execute, em um dos seus projetos, o comando **git diff HEAD~1 HEAD** e certifique-se de que entende o resultado apresentado.
