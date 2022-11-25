# COMANDOS DE ARQUIVOS
___

- **ls** - listagem de diretório
- **ls -la**  - listagem formatada   de diretórios com arquivos ocultos
- **cd *dir*** - muda diretório para *dir*
- **cd** - muda para o *home*
- **pwd** - mostra o diretório atual
- **mkdir *dir*** - cria o diretório *dir*
- **rm *arquivo*** - exclui *arquivo*
- **rm*** - exclui todos os diretórios ***(Cuidado)***
- **rm -r *dir*** - exclui o diretório *dir*
- **rm -f *arquivo*** - força remoção de *arquivo* ***(Cuidado)***
- **rm -rf *dir*** - força a remoçaõ do diretório *dir* ***(Cuidado)***
- **cp *arq1 arq2*** - copia *arq1* para *arq2*
- **cp -r *dir1 dir2*** - copia *dir1* para *dir2*; cria*dir2 se não existir*
- **mv *arq1 arq2*** - renomeia ou move *arq1* para *arq2*, se *arq2* é um diretório existente, move *arq1* dentro do diretório *arq2*
- **ln -s *arquivo* link** - cria uma ligação simbólica *link* para o arquivo
- **touch *arquivo*** - cria atualiza *arquivo*
- **cat > *arquivo*** - coloca entrada padrão em *arquivo*
- **more *arquivo*** - conteúdo de *arquivo* com pausa
- **head *arquivo*** - primeiras 10 linhas de *arquivo*
- **tail *arquivo*** - últimas 10 linhas de *arquivo*
- **tail -n** - mostra um número determinados de linhas
- **tail -f *arquivo*** - conteúdo do *arquivo* conforme ele cresce, começando com as 10 últimas
- **echo** - imprime o que se escreve
- **history** - mostra os últimos 100 comando 
- **passwd** - atualiza a senha
- **passwd -d** - cria um novo usuário sem senha
- **wc** - mostra o tamanho dos arquivos
- **cut** - delimita o que será mostrado
- **sort** - organisa o mostra os arquivos
- **unic** - mostra unicamente o arquivo
- **more** - cria uma barra de rolagem
- **last** - movimenta a tela com bara de rolagem
- **man** - manual para arquivos e comandos
- **ls > *arquivo*** - envia uma saída de dados para a pasta *arquivo*, reescreve sobre o conteúdo anterior
- **ls >> *arquivo*** - envia uma saída de dados para a pasta *arquivo*, acrescentando ao conteúdo anterior
- **>file.txt** - cria uma arquivo vazio, semelhante ao **touch**
- **&** - executa o software em background
- **&&** - se a ação anterior for bem sucedida, executa a ação adicional
    ex: ls aaa && >file a
- **||** - somente executa o 2º comando se o 1º não tiver exito
- **;** - executa o 2º comando se o 1º comando for bem sussedido ou não
- **>** - mostra a entreda de um arquivo
- **-** - envia sdtout para stdin do outro comando

# Gerenciamento de Processos
___

- **ps** - mostra seus processos  ativos
- **top - m** - mostra todos os processos rodando
- **kill *pid*** - mata o processo com id *pid*
- **killall - *proc*** - mata todos os processos chamados *proc**
- **bg** - lista todos os trabalhos parados ou em *background*; prossegue um trabalho parado em background
- **fg** - traz o trabalho mais recente para *foreground*
- **fg n** -traz o trabalho *n* para foreground 


# Permissões de Arquivo
___

- **chmod octal *arquivo*** - altera as permissões do arquivo paraoctal, separadamente para usuário, grupo e mundo, adicionando:
    - 4 - read (r)
    - 2 - write(w)
    - 1 - execute(x)

Exemplos:
- **chmod 777** - read, write, execute para todos
- **chmod 755** - rwx para proprietário, rx para grupo e mundo

Para mais opções, **man chmod**

# SSH
___

**ssh *user@host*** - conecta no *host* como user
**ssh -p *porta* user@host** - conecta no *host* na *porta* como user
**ssh-copy-id *user@host*** - adiciona sua chave ao host para *user* para permitir login com chave (passwordless)


# Pesquisa
___

- grep padrão *arquivos* - pesquisa pelo *padrão* nos arquivos
- grep -r padrão diretório - pesquisa recursivamente pelo padrão no diretório
- grep -rni - pessquisa em todas as pastas
- comando | grep padrão - pesquisa pelo padrão na saída do comando
- locate arquivo - pesquisa todas as instâncias de arquivo

# Informações do Sistema
___

- **date** - mostra a data/hora atuais
- **cal** - mostra calendário mensal
- **uptime** - tempo que o sistema etá aberto
- **w** - mostra quem etá *online*
- **whoami** - mostra o usuário atual
- **finger *user*** - informações sobre *user*
- **uname -a** - mostra informações sobre o Kernel
- **cat /proc/cpinfo** - informações da cpu
- **cat /proc/meminfo** - informações da memória
- **man *comando*** - mostra o manual para o *comando*
- **df** - mostra o uso so disco
- **du** - mostra espaço em uso no diretório
- **free** - mostra uso da memóriae aréa de *swap*
- **whereis app** - possível localização de *app*
- **which *app*** - mostra qual *app* será executada por padrão


# Compressão
___

- **tar cf arq.tar *arquivos*** - cria um tar chamado arq.tar contendo *arquivos*
- **tar xf arq.tar** - extraí os arquivos de arq.tar
- **tar czf arq.tar.gz files** - cria um tar dom compressão Gzip
- **tar xzf *file*.tar.gz** - extraí um tar usando Gzip
- **tar cjf *file*.tar.bz2** - cria um tar usando compressão Bzip2
- **tar xjf *file*.tar.bz2** - extraí um tar usando Bzip2
- **gzip *arquivo*** - comprime *arquivo* e renomeia para *arquivo.gz*
- **gzip -d *arquivo.gz*** - descompacta file.gz de volta para *arquivo*


# Rede
___

- **ping *host*** - pinga o *host* e mostra resultados
- **whois *domínio*** - pega informações *whois* para o *domínio*
- **dig *dominio*** - pega informações DNS do do *domínio*
- **dig -x host** - DNS reverso
- **wget *arquivo*** - baixa *arquivo*
- **wgt -c *file*** - continua um download parado


# Instalação
___

-  Instalação a partir dos fontes:
-  **./configure**
-  **make**
-  **make install**
-  **dpkg -i pkg.deb** - instala um pacote (Debian)
-  **rpm - Uvh pkg.rpm** - instala um pacote (RPM)


# Atalhos
___

- **Ctrl + c** - finaliza o comando atual
- **Ctrl + z** - interrompe o comando atual, mas permite recomeçar com **fg** (em foreground) ou **bg** (background)
- **Ctrl + d** - encerra a sessão atual, similar a **exit**
- **Ctrl + w** - apaga uma palavra na linha atual
- **Ctrl + u** - apaga a linha inteira
- **Ctrl + r** - apresenta um comando recente
- **Ctrl + a** - vai para o inicío da linha
- **Ctrl + e** - vai para o final da linha
- **Ctrl + u** corta do cursor para traz
- **!!** - repete o ultimo comando usado
- **exit** - abandona a sessão atual

