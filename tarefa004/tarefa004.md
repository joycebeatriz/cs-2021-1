<p style="text-align: center;"><font size="4"><b>Git <i>branching</i> [Exercícios]</b></font></p1></p>
<DIV align="justify">

1. Qual o nome do branch padrão do Git?
<pre> master </pre> 

2. O que o comando **<code>git branch nome</code>** realiza
<pre> cria um branch com o nome escolhido. </pre>

3. Como criar um branch a partir de um commit específico?
<pre> git branch</pre>   

4. Em um repositório, qual o efeito do comando **<code>git checkout -b bugfix/234</code>**?
<pre> cria um novo branch com o nome erro1234 que ficara junto com master.</pre>   

5. Qual o comando para se alternar para um branch de nome **experimento2**?
<pre> git checkout experimento2.</pre>    

6. Em um repositório com dois branches, **b1** e **b2**, onde b1 é o corrente, qual o efeito do comando **<code>git branch</code>**?
 <pre> apareceria as duas branch no terminal, no entanto, a b1 estaria destacada de verde com um "*", para demonstrar qual é a principal.</pre>     

7. O que o comando **<code>git checkout -b</code>** nome faz?
<pre> cria uma nova branch e a torna como branch principal.</pre>    

8. Qual a função do <code>**comando git branch -d teste</code>**?
<pre> exclui a branch teste.</pre>  

9.  Durante o desenvolvimento de um software é comum, por exemplo, utilizar um novo recurso por meio de experimentação. Talvez uma nova tecnologia, uma nova biblioteca que pode ser útil ao que está em desenvolvimento, ou até mesmo uma nova versão de um produto já empregado. Para que o uso deste novo recurso não interfira com o que é considerado pronto, um branch pode ser criado para a experimentação. Código que for criado para a experimentação existirá apenas no branch criado. Se eventualmente o experimento demonstrar um resultado satisfatório, as alterações realizadas no branch poderão ser incorporadas no que é considerado pronto, ou seja, no branch principal (master). Esta última ação é conhecida por merge. Neste item, crie uma sequência de comandos que simula um caso simples de criação e uso seguido de merge empregando um branch para ilustrar uma experimentação conforme acima. A sequência deve incluir, obrigatoriamente: (a) criação de um ou mais branches; (b) chaveamento para pelo menos dois branches e (c) merge.

<pre>  
        git branch aluno
        git branch professor 
        git checkout aluno 
        git checkout professor
        arquivo teste.md é criado 
        git add teste.md 
        git commit
        arquivo alterado teste.md 
        git add -u 
        git commit "modificação do arquivo teste.md"
        git checkout master 
        git merge aluno
        git merge professor 
</pre>  


</DIV/>