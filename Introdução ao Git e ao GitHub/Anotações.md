# Navegação básica no terminal e instalação

comandos:  
Windows		Linux 		Função  
dir		ls		listar conteúdo  
cd 		cd		navegação  
cd..		cd..		retorna um nível  
cls		clear (Ctrl+L)	limpar tela   
TAB		TAB		autocompletar   
mkdir		mkdir		criar pasta   
del				deleta arquivo   
rmdir		rm -rf		remove todo diretório   


# Entendendo como Git funciona

sha1 -> secure hash algorithm -> NSA  
Gera um conjunto de caracteres identificador de 40 dígitos.  
openssl sha1 ******.txt  

# Objetos internos do Git

Blob -> Contém metadados: tipo, tamanho, etc.   
Tree -> Aponta para um blob ou outras tree. Guarda o nome do arquivo, tamanho, tipo, etc(metadados). Se houver mudança em qualquer arquivo em que a tree aponta o sha1 irá mudar.   
Commit -> O sha1 desse commit é o hash de toda a informação. Guarda o tamanho, tree, parent, autor, mensagem e timestamp.   
GIT -> Sistema distribuido e seguro   

# Chaves SSH e Tokens

Chave ssh -> Forma de estabelecer uma conexão segura entre o servidor e a máquina local. Sempre vai ter uma chave pública e uma particular.   
Token -> Similar a usuário e senha, mas é necessário inserir o token em vez da senha parar autenticar. No token usa https para clonar no terminal    

# Iniciando o Git e criando um commit

git init -> cria um repositório  
.git -> pasta gerencial do git (fica todos os objetos, etc).   

Antes de inicializar o git é necessário configurações iniciais    
git config --global user.email "***********"   
git config --global user.name "**********"   

Arquivo Markdown (*.md) -> similar ao html usa tags mais humanizadas.   
git add * -> adiciona arquivos ou pastas para o stage   
git commit -m "descrição" -> cria um commit    

# Ciclo de vida dos arquivos no Git

git status -> estado do arquivo   
git remote add origin *************** (local para remoto)   
git push origin main    

# Resolvendo conflitos

git clone "**************"   
git pull origin main   


