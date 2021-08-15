# AtividadeRemota
Atividade Remota - SENAI-SP

Esta é uma proposta de solução para a Atividade Remota
•	Criaremos uma demanda de times cariocas, identificados no arquivo ClubesCariocas.txt para participar da relação de times do torneio, inseridos no arquivo CampeonatoCarioca.txt.
•	Existirá uma relação de clubes que não pertencem ao campeonato carioca e estão descritos no arquivo ignorado denominado ClubesDeOutrosEstados.txt.
•	Diferentemente da Atividade 1, esta insere a possibilidade de colaboração com mais desenvolvedor B, responsável por alterar/modificar o arquivo de times para o torneio Rio-Bahia de futebol, permitindo o acesso ao novo arquivo, Torneio_Rio-Bahia.txt, e a inserção de clubes de futebol bahiano para o match.
Atividade Remota      -        Step by Step
1.	 Instalamos o software GitHub 2.32.0.windows.2 baixado do site http://git-scm.com para Windows 10 32 bits com as ferramentas Git GUI e Git Bash embutidas.
2.	Habilitamos o View de Explorer de Windows a exibir explicitamente as extensões dos arquivos armazenados nas pastas bem como aqueles ocultos.
3.	Criamos o diretório AtividadeRemota no Desktop e nos posicionamos nele.
4.	Confirmamos a versão instalada do Git com o comando
a.	git –version
git version 2.32.0.windows.2
5.	Nos posicionamos no diretório AtividadeRemota e emitimos o comando
a.	git init para criar o repositório   .git   sob o diretório corrente Atividade 1
6.	Criamos os arquivos:
a.	ClubesCariocas.txt com os nomes dos principais clubes de futebol do Rio de Janeiro
b.	ClubesDeOutrosEstados.txt com alguns nomes de clubes de outros estados
c.	CampeonatoCarioca.txt  com os mesmos clubes cariocas
d.	Torneio_Rio-Bahia, inicialmente com os clubes cariocas apenas e nenhum de outros estados
7.	Criamos o arquivo .gitignore e inserimos neste o nome do arquivo ClubesDeOutrosEstados.txt para ser ignorado pelo git. E que agora não possui clubes baianos.
8.	Emitimos o comando 
a.	git status para verificar os arquivos ainda rastreáveis pelo git (aparecem em vermelho)
9.	Configuramos duas das variáveis globais para fins de comunicação futura com o GitHub.com:
a.	git config - -global user.name   “Antonio-Adilson”
b.	git config - -global user.email   “a2f_adler@yahoo.com”
10.	A seguir, emitimos o comando
a.	git add . para adicionar todos os arquivos ainda não monitoráveis ao monitoramento
11.	Então, emitimos o comando
a.	git commit - que finaliza arquivos depois de adicionados para o monitoramento. Snapshot
12.	Emitimos o comando 
a.	git status para verificar se estava tudo ok e fomos bem sucedidos
Outros comandos úteis a serem explorados: 

LISTA DE TODOS OS COMANDOS GIT


•	git init – cria o repositório no diretório selecionado.
•	ls – mostra conteúdo.
•	git status – mostra o estado em que estão os arquivos, caso rastreados ou não.
•	.gitignore – arquivo criado para adicionar arquivos para serem ignorados.
•	git config user.name “” – adiciona nome do desenvolvedor. Caso --global não é apenas local.
•	git config user.email “” – adiciona email do desenvolvedor.
•	git add nomedoarquivo. – adiciona o arquivo para o monitoramento. Tracked.
•	git commit -m “” – finaliza arquivos depois de adicionados para o monitoramento. Snapshot.
•	modified – arquivo no monitoramento que é modificado e salvo. git add para atualizar.
•	git log – mostra todo o histórico das ações no git. Mostra usuário e id.
•	git config core.pager cat – adiciona configuração no repositório para log.
•	git log -número – os últimos mostrados na numeração.
•	git log --oneline – informações de log em uma linha. Id e mensagem.
•	git log --before “XXXX-XX-XX” – mostra log anterior a data escolhida.
•	git log --after “XXXX-XX-XX” – mostra log após a data escolhida.
•	git log --since=“n days ago” – mostra log de dias atrás.
•	q – sai do log.
•	git checkout id – sete primeiros dígitos do commit. Vai para o commit do id.
•	git checkout master – volta para a cabeça.
•	git show – mostra informações do último commit.
•	git remote -v – apresenta o nome do repositório.
•	git push origin – manda para o repositório original.
•	git branch -a – mostra todas as branchs incluindo remotas.
•	git fetch – recolhe as branchs.
•	git push origin nomedabranch – encaminha para o repostitório remoto a branch adicionada.
•	git push origin nomedoarquivo – encaminha o arquivo para o repositório.
•	git mv nomedoarquivo novonome – renomear arquivos.
•	git rm nomedoarquivo – remove arquivo do repositório. Pode ser commitado.
•	git diff --staged – compara arquivo em staged com a última versão do commit.
•	git diff id – compara o do id com o último commit.
•	git diff id..id – compara todos os ids entre os colocados, dó último para o mais novo.
•	git commit --amend -m “” – corrigindo mensagem. Adiciona arquivo no último commit.
•	git restore --staged nomedoarquivo – retira arquivo do add, monitoramento.
•	git checkout nomedoarquivo – retorna para a versão anterior do arquivo modificado.
•	git reset HEAD --hard – sobrescreve todos os arquivos retirando últimas alterações.
•	git reset HEAD^ --hard – volta para o ultimo commit.
•	git branch – exibe todos os branchs.
•	git branch nomedobranch – cria um novo branch.
•	git checkout nomedobranch – muda para o outro branch.
•	git branch -d nomedobranch – deleta o branch. D para confirmar.
•	git merge nomedobrach – une o branch com o principal.
•	git checkout -b novobranch – cria e muda para novo branch.
•	git rebase nomedobranch – une arquivos com o branch main.
•	pwd – mostra o home.
•	git clone home – clona o endereço home de um repositório para diretório de colaborador.
•	ls -la – mostra os arquivos ocultos.
•	touch nomedoarquivo – cria o novo arquivo no novo diretório.
•	git push – encaminha o diretório para o repositório original. Para Bare-repository.
•	git fetch – baixa os arquivos para o diretório trabalhado.
•	git rebase – o novo arquivo é adicionado.
•	git pull – encaminha os arquivos para o repositório remoto.
•	git init --bare – cria repositório vazio.
•	git clone endereçohome-bare . – clona repositório vazio.
•	cat config – mostra informações de configuração do repositório.
•	cd nomedapasta – acessa a pasta.
•	git tag nomedatag (ex v1.0) – cria uma tag que pode ser o projeto final.
•	git tag – mostra as tags existentes no repositório.
•	git push origin nomedatag – no repostiório da tag encaminha a tag para repositório remoto.
•	git checkout nomedatag – muda para a tag escolhida.
•	git switch -c nomedabrachtag – vai para o branch da tag. Merge e push origin para nova tag.
•	git remote add origin endereçodorepositórioremoto – para adicionar repositório github.
•	git push -u origin nomedobranch – adiciona repositório local para remoto.
•	git config credential.helper store – adiciona nova credencial para o projeto para push.
•	git clone endereçodoprojetogithub – clona o projeto para o novo repositório.
•	git pull origin master – atualizar projeto a partir do branch principal.
•	git checkout -- . – volta os arquivos ao estado original.
•	gti checkout – nomedoarquivo – volta o arquivo a versão antes da modificação.l
•	git add . – adiciona todos os arquivos ao staged.
•	git checkout HEAD -- . – volta todos os arquivos ao estágio anterior.
•	git revert id – cria novo commit removendo o que foi modificado no arquivo.
•	git push -u origin master – adiciona arquivos para o branch principal.
•	git reset – remove o commit.
•	git reset HEAD~-numeração – numeração de quantos commits devem ser resetados.

