## **Os Principais comandos do Git**

Quando eu estudo, eu gosto de sempre anotar as coisas que estou aprendendo, para que eu consiga absorver melhor. Então, eu  listarei aqui os principais comandos do Git que eu encontrei.



###  Git Clone

Este comando serve para fazer uma cópia idêntica e baixar um repositório que está localizado na internet (em serviços como o GitHub). 

Exemplo de linha digitada no Git:

*git clone <https://nomedosite.com.br>*



### Git Branch

Os branches fazem com que múltiplos devs trabalhem ao mesmo tempo no mesmo projeto. Podemos usar esse comando para criar, listar ou deletar branches. 

- Para criar um novo branch, basta digitar o comando:

*git branch <nome-do-branch>*

Para visualizar branches, o comando é:

*git branch --list*

E para deletar um brach, escreva:

*git  branch -d <nome-do-branch>*



### Git Status

Este comando nos mostra o estado atual do branch e também nos dá todas as informações que precisamos. 

O comando é:

*git status*



### Git Add

Quando nós criamos, modificamos ou deletamos um arquivo, essas mudanças acontecem apenas na nossa máquina local e não serão incluídas no próximo commit, a não ser que adicionemos essas mudanças. 

Para incluir apenas um arquivo, use o comando:

*git add <arquivo>

Para adicionar tudo de uma vez:

*git add -A*



### Git Commit

Quando atingimos um certo ponto do nosso projeto, é bom salvar todas as alterações feitas até o momento. O comando commit é como um "checkpoint", ou seja, se eu cometer algum erro, ou perder os dados, eu posso voltar exatamente naquele ponto onde eu salvei. Por isso, esse é um dos comandos mais usados no Git. É importante também adicionar uma mensagem a cada comando Commit, para que a gente possa lembrar o que fizemos, ou para que outra pessoa possa entender o que foi feito também.

Para usar esse comando, digite:

*git commit -m "mensagem"*



### Git Push

Depois de todas as alterações feitas, o próximo passo é fazer o upload delas para o servidor na internet. O comando push faz o upload de todas as alterações e arquivos novos para o seu repositório online, fazendo com que os repositórios local e online estejam iguais. 

O comando para fazer o upload é:

*git push <remoto> <nome-do-branch>*



### Git Pull

Este comanto é o oposto do Git Push, ou seja, através desse comando, vc faz o download das alterações feitas no repositório online para sua máquina local. 

O comando é:

*git pull <remote>*



### git Revert

As vezes, precisamos reverter as mudanças que fizemos. Então, esse comando faz exatamente isso, apaga a última alteração que você fez, e por isso esse comando deve ser usado com caltela, pois você pode deletar alguma coisa que não queria. O ideal, é que você veja quais foram as últimas alterações, para ter certeza daquilo que quer reverter. Um jeito fácil de visualizar, é utilizar o comando *git log --oneline*, depois de ver o que precisa ser revertido, basta usar o comando de reverter junto com o hash code.

Exemplo:

*git revert 254856*



