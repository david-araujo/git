CONFIGURAÇÕES INICIAIS:

git config = Comando utilizado para setar configurações no git globalmente ou em um determinado projeto.
OBS: Para setar configurações Globais utilizamos a diretiva --global

Setar Nome: git config user.name "SEU_NOME" OU git config --global ...
Setar Email: git config user.email "SEU@EMAIL.com"

Listar suas configurações iniciais:
    Individual: git config --global (OPCIONAL) user.name OU ...user.email
    Todo o conteudo:
        git config --global --list

    Utilizando comando cat do Linux:
        cat ~/.gitconfig

    Podemos também alterar o arquivo .gitconfig em qualquer editor.

    Podemos abilitar uma interface colorida e mais amigavel:
        git config --global color.ui true

!IMPORTANTE:
    Muitas vezes trabalhamos com times em que cada integrante utiliza um Sistema Operacional diferente. Neste caso podemos nos defrontar com carcters returns "ENTER", que possuem códigos diferentes em cada SO.

    Sendo assim podemos configurar o git para remover estes caracteres e postar somente o conteudo alterado no projeto.

        WINDOWS:  git config --global core.autocrlf true
        LINUX: git config --global core.autocrlf input

--------------------------------------------------------------------------------

CONFIGURANDO ALIAS:

ALIAS funcionam como atalhos para comandos.
    EX: git status -s
    Criaremos um Alias que funcionará da mesma maneira que o exemplo acima.

        git config --global alias.s "status -s"

        Agora basta digitar git s ao invés de git status -s

    DICA: Crie um alias muito util de log:
        git config --global alias.lg "log --oneline --all --graph --decorate"

Veremos mais adiante como os comandos funcionam e etc. Sendo assim é hora de conhecermos a fundo o GIT.
