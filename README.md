# GitScript
Script Git for clone subdirectories

## Run de following comands (Powershell ^7 or Bash)

### Criar um diretório, para o Git não ficar bagunçado, e entrar no mesmo.
```ps1 
mkdir (comando para receber o local onde deve ser criada a pasta do projeto) && cd (pasta do projeto)
```
### Iniciar um repositório Git.
```ps1 
git init (iniciar na pasta previamente informada no primeiro comando)
```
### Rastrear o repositório, não informe o subdiretório.
```ps1 
git remote add -f origin github.link
```
### Ativar o recurso de verificação em árvore.
```ps1 
git config core.sparseCheckout true
```
### Informe apenas o subdiretório entre os ' '.
```ps1 
echo 'subdiretório' >> .git/info/sparse-checkout
```
### Fazer o download com o pull e não com o clone (Observe a Branch certa do repositório!)
```ps1 
git pull origin master
```
