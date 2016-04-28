GIT COMANDS

STATUS:
Mostra todos os arquivos que estão prontos para serem comitados e que não estão trakeados

    git status


--------------------------------------------------------------------------------

ADD:
Adiciona os arquivos a stage area (Trakea os arquivos).

    git add NOME_DO_ARQUIVO
    git add . = Adiciona todos os arquivos que não foram trackeados.
    git add * = Trackea arquivos com determianada combinação
    -A ou --all = Trekea todos os arquivos incluindo os que devem ser deletados.

--------------------------------------------------------------------------------

COMMIT:
Empacota os arquivos e os prepara para serem enviados para o servidor ou para o GitHub.

    git commit -m "MENSAGEM DE HISTÓRICO"

OBS: Ao dar um commit SEMPRE utilize a diretiva -m para não ser requisitado mais tarde.

--------------------------------------------------------------------------------
LOG:
Lista todos os commits relizados em detalhes.
    git log
        --oneline = Exibe ID do commit e mensagem.
        --decorate = Mostra qual o ultimo commit realizado e branch

            Uma boa pratica é criar um Alias git lg
            git config alias.lg "log --oneline --decorate"
            
--------------------------------------------------------------------------------
