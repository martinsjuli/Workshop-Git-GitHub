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
Acesse a pasta que deseja transformar em um repositório Git  pelo terminal ou clique no atalho em “Git Bash Here”:
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
4. Adiciona uma alteração no diretório de trabalho para a área de preparação . Ele informa ao Git que você deseja incluir atualizações no próximo commit:
    ```bash
    git add . 
    ```
4. Commits podem ser considerados como instantâneos ou marcos ao longo do cronograma de um projeto Git. Commits são criados com o comando git commit para capturar o estado de um projeto naquele ponto no tempo:
    ```bash
    git commit -m "Mensagem" 
    ```    
##

### Desfazendo Alterações no Repositório Local

#### Como alterar a mensagem do último commit
```bash
git commit --amend
```
Alterando a mensagem sem abrir o editor:  
```bash
git commit --amend –m"nova mensagem"
```

#### Como desfazer um commit
```bash
git reset
```
```bash
git reset --soft
```
```bash
git reset --mixed
```
```bash
git reset --hard
```

##
<div align="center">Feito com 💙 por <a href="https://github.com/jocarsbarsa">João Carlos</a>.</div>
