1)	Criar um repositório público denominado “exercicio01”:
@TiagoALira ➜ /workspaces/codespaces-blank $ git config --global user.name "Tiago Lira"
@TiagoALira ➜ /workspaces/codespaces-blank $ git config --global user.email "tiago.lira@faculdadeimpacta.com.br"
@TiagoALira ➜ /workspaces/codespaces-blank $ mkdir exercicio01
@TiagoALira ➜ /workspaces/codespaces-blank $ cd exercicio01/
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 $ git init

2)	Criar um arquivo na raiz principal (main) chamado “README.md”
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo exercicio01 > README.md
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ ls
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

3)	Etapas da prática na Aula 02 (Básico sobre staging / commit):

a) No working dir, executar o comando: echo 01 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ ls
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat arquivo.txt

b) Adicionar o arquivo no staging e conferir o status
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

c) Commitar o arquivo do staging com a descrição "git add example - arquivo.txt“
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add example - arquivo.txt"
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

d) Sobrescrever o conteúdo do arquivo.txt: echo 02 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat arquivo.txt

e) Verificar o diffing no arquivo
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff

f) Adicionar novamente o arquivo no staging e conferir o status
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

g) Verificar o diffing no arquivo
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

h) Sobrescrever o conteúdo do arquivo.txt: echo 03 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

i) Verificar o diffing no arquivo
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff

j) Fazer o restore do arquivo da área de staging e verificar o status
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore arquivo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status

k) Realizar o commit do arquivo e verificar o log
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "Commit Arquivo.txt"

l) Adicionar um arquivo gitignore com o seguinte conteúdo: *.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat .gitignore

m) Criar um arquivo novo.txt e verificar o status
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo > novo.txt
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ ls
@TiagoALira ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
