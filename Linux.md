# COMANDOS DE ARQUIVOS

- **ls** - listagem de diretório
- **ls -la**  - listagem formatada   de diretórios com arquivos ocultos
- **cd *dir*** - muda diretório para *dir*
- **cd** - muda para o *home*
- **pwd** - mostra o diretório atual
- **mkdir *dir*** - cria o diretório *dir*
- **rm *arquivo*** - exclui *arquivo*
- **rm*** - (Cuidado) exclui todos os diretórios
- **rm -r *dir*** - exclui o diretório *dir*
- **rm -f *arquivo*** - força remoção de *arquivo*
- **rm -rf *dir*** - força a remoçaõ do diretório *dir*
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
- **whoami** - mostra o usuário atual
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



# Gerenciamento de Processos

- **ps** - mostra seus processos  ativos
- **top - m** - mostra todos os processos rodando
- **kill *pid*** - mata o processo com id *pid*
- **killall - *proc*** - mata todos os processos chamados *proc**
- **bg** - lista todos os trabalhos parados ou em *background*; prossegue um trabalho parado em background
- **fg** - traz o trabalho mais recente para *foreground*
- **fg n** -traz o trabalho *n* para foreground 

# Permissões de Arquivo

- **chmod octal *arquivo*** - altera as permissões do arquivo paraoctal, separadamente para usuário, grupo e mundo, adicionando:
    - 4 - read (r)
    - 2 - write(w)
    - 1 - execute(x)

Exemplos:
- **chmod 777** - read, write, execute para todos
- **chmod 755** - rwx para proprietário, rx para grupo e mundo

Para mais opções, **man chmod**

# SSH

# Pesquisa

# Informações do Sistema

# Compressão

# Rede

# Instalação

# Atalhos