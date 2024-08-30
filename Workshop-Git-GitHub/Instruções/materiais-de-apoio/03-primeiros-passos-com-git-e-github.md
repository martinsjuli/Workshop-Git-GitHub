<h1>
    <a href="https://javanoroeste.com.br/javanoroeste/">
     <img align="center" width="40px" src="https://javanoroeste.com.br/javanoroeste/javaday_riopreto/favicon.svg"></a>
    <span> Versionamento de Código com Git e GitHub</span>
</h1>

## Primeiros Passos com Git e GitHub

### Criando e Clonando Repositórios
Existem duas formas de obter um repositório Git na sua máquina:
1. Transformando um diretório local que não está sob controle de versão, num repositório Git;
2. Clonando um repositório Git existente.

#### Criando um Repositório Local
Acesse a pasta que deseja transformar em um repositório Git pelo terminal ou clique no atalho em “Git Bash Here”:
1. Inicialize um repositório Git no diretório escolhido:
    ```bash
    git init
    ```
2. Conecte o repositório local com o repositório remoto:
    ```bash
    git remote add origin https://github.com/username/nome-do-repositorio.git
    ```
3. Visualizar alterações:
    ```bash
    git status
    ```

### Trabalhando com Branches

#### Criando e Mudando para uma Nova Branch
Antes de começar a trabalhar em um novo recurso ou correção de bug, é uma boa prática criar uma nova branch. Para criar uma nova branch e alternar para ela, use:
```bash
git checkout -b nome-da-branch

###Listando Branches
Para listar todas as branches em seu repositório e ver em qual você está atualmente, use:
```bash
git branch
```
###Mudando para Outra Branch
Para mudar para uma branch existente, use:
```bash
git checkout nome-da-branch
```

####Adicionando Mudanças e Committing
4. Adicione uma alteração no diretório de trabalho para a área de preparação. Isso informa ao Git que você deseja incluir atualizações no próximo commit:
```bash
git add .
```

5. Commits podem ser considerados como instantâneos ou marcos ao longo do cronograma de um projeto Git. Commits são criados com o comando git commit para capturar o estado de um projeto naquele ponto no tempo:
```bash
git commit -m "Mensagem" 
```

###Enviando Alterações para o Repositório Remoto
####Puxando Alterações do Repositório Remoto
6. Antes de enviar suas alterações, é uma boa prática puxar as alterações do repositório remoto para garantir que sua branch local esteja atualizada:
```bash
git pull origin nome-da-branch
```
####Enviando Commits para o Repositório Remoto
7. Depois de ter feito commit de suas alterações, você pode enviá-las para o repositório remoto:
```bash
git push origin nome-da-branch
```

###Desfazendo Alterações no Repositório Local
Como alterar a mensagem do último commit
```bash
git commit --amend -m "Nova Mensagem"
```

####Como desfazer um commit
8. Reverte o último commit, mantendo as alterações:
```bash
git reset --soft HEAD~1
```
Reverte o último commit e as alterações voltam para a área de staging:
```bash
git reset --mixed HEAD~1
```
Reverte o último commit e descarta as alterações:
```bash
git reset --hard HEAD~1
```

####Como excluir uma branch
9. Exclua uma branch que não é mais necessária:
```bash
git branch -d nome-da-branch
```

10. ####Conclusão
Seguindo esses passos, você conseguirá gerenciar o versionamento de código de maneira eficaz usando Git e GitHub. Lembre-se sempre de confirmar se a branch na qual você está trabalhando é a correta e de comunicar bem com sua equipe sobre as alterações e merges.
##
<div align="center">Feito com 💙 por <a href="https://github.com/jocarsbarsa">João Carlos</a>.</div>
