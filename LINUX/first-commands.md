# Comandos Linux:

## 1. `cd` (Change Directory)
**Significado:** Mudar de diretório.

- **Opções:** 
  - `cd -` (volta para o diretório anterior)
  - `cd /` (vai para o diretório raiz)
  - `cd ~` (vai para o diretório home)
  
- **Exemplos de uso:**
  - `cd /home/usuario` (muda para o diretório do usuário)
  - `cd ..` (volta um nível no diretório atual)
  - `cd -` (volta para o último diretório acessado)
  - `cd /` (vai para a raiz do sistema)
  - `cd ~` (é a mesma coisa que fazer `cd /home/usuario`)

---

## 2. `mv` (Move)
**Significado:** Mover ou renomear arquivos/diretórios.

**Sintaxe**
`mv [opções] origem destino`

- **Opções:**
  - `mv -i` (pede confirmação antes de sobrescrever)
  - `mv -v` (exibe detalhes da operação)
  - `mv -n` (não sobrescreve arquivos existentes)

- **Exemplos de uso:**
  - `mv arquivo.txt /home/usuario/Documentos` (move arquivo.txt para o diretório Documentos)
  - `mv arquivo_antigo.txt arquivo_novo.txt` (renomeia arquivo_antigo.txt para arquivo_novo.txt)
  - `mv -i arquivo.txt /home/usuario/Documentos` (pede confirmação antes de mover o arquivo se já houver um arquivo com o mesmo nome)
  - `mv -v arquivo.txt /home/usuario/Documentos` (mostra detalhes da movimentação)
  - `mv -n arquivo.txt /home/usuario/Documentos` (não sobrescreve um arquivo existente)

---

## 3. `cp` (Copy)
**Significado:** Copiar arquivos/diretórios.

**Sintaxe**
`cp [opções] origem destino`

- **Opções:**
  - `cp -r` (copia diretórios recursivamente)
  - `cp -i` (pede confirmação antes de sobrescrever)
  - `cp -v` (exibe detalhes da operação)
  - `cp -p` (mantém permissões e timestamps)

- **Exemplos de uso:**
  - `cp arquivo.txt /home/usuario/Documentos` (copia arquivo.txt para o diretório Documentos)
  - `cp -r pasta1/ pasta2/` (copia a pasta1 e seu conteúdo para pasta2)
  - `cp -i arquivo.txt /home/usuario/Documentos` (pede confirmação antes de sobrescrever)
  - `cp -v arquivo.txt /home/usuario/Documentos` (mostra detalhes da cópia)
  - `cp -p arquivo.txt /home/usuario/Documentos` (mantém permissões e timestamps originais)

---

## 4. `ls` (List)
**Significado:** Listar arquivos e diretórios.

**Sintaxe**
`ls [opções] [caminho]`

- **Opções:**
  - `ls -l` (exibe detalhes como permissões, proprietário, tamanho e data)
  - `ls -a` (lista todos os arquivos, incluindo ocultos)
  - `ls -h` (exibe o tamanho de forma legível, como KB, MB)
  - `ls -t` (ordena pela data de modificação mais recente)
  - `ls -r` (ordena a lista em ordem reversa)
  - `ls -R` (lista recursivamente subdiretórios)

- **Exemplos de uso:**
  - `ls` (lista arquivos no diretório atual)
  - `ls -l` (lista arquivos com detalhes)
  - `ls -a` (lista todos os arquivos, incluindo ocultos)
  - `ls -lh` (lista arquivos com detalhes e tamanhos legíveis)
  - `ls -lt` (lista arquivos ordenados pela data de modificação)
  - `ls -la` (lista todos os arquivos, incluindo ocultos, com detalhes)
  - `ls -R` (lista arquivos e subdiretórios recursivamente)

---

## 5. `grep` (Global Regular Expression Print)
**Significado:** Filtrar texto usando expressões regulares.

**Sintaxe**
`grep [opções] 'padrão' [arquivo(s)]`

- **Opções:**
  - `grep -i` (ignora diferenças de maiúsculas/minúsculas)
  - `grep -v` (exibe linhas que não correspondem ao padrão)
  - `grep -r` (procura recursivamente em diretórios)
  - `grep -l` (exibe somente os nomes dos arquivos que contêm correspondências)

- **Exemplos de uso:**
  - `grep "texto" arquivo.txt` (procura "texto" em arquivo.txt)
  - `grep -i "texto" arquivo.txt` (procura "texto" ignorando maiúsculas/minúsculas)
  - `grep -v "erro" arquivo.log` (exibe linhas que não contêm a palavra "erro")
  - `grep -r "erro" /var/log` (procura recursivamente por "erro" na pasta /var/log)
  - `grep -l "texto" *` (exibe o nome dos arquivos que contêm a palavra "texto")

---

## 6. `tail`
**Significado:** Exibir as últimas linhas de um arquivo.

**Sintaxe**
`tail [opções] [arquivo]`

- **Opções:**
  - `tail -n` (define o número de linhas a exibir)
  - `tail -f` (segue a atualização do arquivo em tempo real)
  - `tail -v` (exibe o nome do arquivo antes de mostrar o conteúdo)

- **Exemplos de uso:**
  - `tail arquivo.txt` (mostra as últimas 10 linhas de arquivo.txt)
  - `tail -n 20 arquivo.txt` (mostra as últimas 20 linhas)
  - `tail -f arquivo.log` (exibe as últimas linhas de um arquivo e segue atualizações em tempo real)

---

## 7. `cat` (Concatenate)
**Significado:** Concatenar e exibir conteúdo de arquivos.

**Sintaxe**
`cat [opções] [arquivo(s)]`

- **Opções:**
  - `cat -n` (numera as linhas)
  - `cat -b` (numera apenas linhas não vazias)
  - `cat -s` (suprime linhas em branco consecutivas)

- **Exemplos de uso:**
  - `cat arquivo.txt` (exibe o conteúdo de arquivo.txt)
  - `cat -n arquivo.txt` (exibe o conteúdo de arquivo.txt numerando as linhas)
  - `cat -b arquivo.txt` (exibe o conteúdo e numera apenas as linhas não vazias)
  - `cat -s arquivo.txt` (suprime múltiplas linhas vazias consecutivas)
  - `cat arquivo1.txt arquivo2.txt > novo_arquivo.txt` (concatena o conteúdo dos arquivos 1 e 2 em um novo arquivo)

---

## 8. `vim` (Vi IMproved)
**Significado:** Editor de texto avançado.

- **Exemplos:**
  - `vim arquivo.txt` (abre arquivo.txt no editor Vim)
  - Dentro do Vim:
    - Pressione `i` para entrar no modo de inserção.
    - `Esc` para sair do modo de inserção.
    - `:wq` para salvar e sair.

---

## 9. `head`
**Significado:** Exibir as primeiras linhas de um arquivo.

**Sintaxe**
`head [opções] [arquivo]`

- **Opções:**
  - `head -n` (define o número de linhas a exibir)
  - `head -v` (exibe o nome do arquivo antes de mostrar o conteúdo)

- **Exemplos de uso:**
  - `head arquivo.txt` (mostra as primeiras 10 linhas de arquivo.txt)
  - `head -n 5 arquivo.txt` (mostra as primeiras 5 linhas)

---

## 10. `ping`
**Significado:** Testar a conectividade entre meu computador e outro host.

**Sintaxe**
`ping [opções] <endereço>`

- **Opções:**
  - `ping -c` (define o número de pacotes a serem enviados)
  - `ping -i` (intervalo de tempo entre pacotes)

- **Exemplos de uso:**
  - `ping google.com` (testa a conectividade com o Google)
  - `ping -c 4 google.com` (envia 4 pacotes)
  - `ping -i 0.5 google.com` (envia pacotes a cada meio segundo)

---

## 11. `netstat` (Network Statistics)
**Significado:** Mostrar conexões de rede e estatísticas.
**Principais funcionalidades do `netstat`:**
    - Exibir conexões de rede ativas.
    - Mostrar estatísticas de rede e informações sobre as interfaces de rede.
    - Listar as tabelas de roteamento.
    - Exibir informações sobre as conexões de escuta.

**Sintaxe**
`netstat [opções]`

- **Opções/Exemplos de uso:**
  - `netstat -a` (mostra todas as conexões e portas de escuta)
  - `netstat -t` (exibe somente conexões TCP)
  - `netstat -u` (exibe somente conexões UDP)
  - `netstat -l` (mostra apenas portas que estão em escuta)
  - `netstat -p` (mostra o ID do processo associado a cada conexão)
  - `netstat -n` (mostra endereços IP e números de porta em vez de resolver nomes)
  - `netstat -r` (exibe a tabela de roteamento)
  - `netstat -s` (exibe estatísticas de rede por protocolo)

---

## 12. `nc` (Netcat)
**Significado:** Ferramenta de rede para leitura e gravação de conexões.

**Sintaxe**
`nc [opções] [hostname] [port]`

- **Opções:**
  - `nc -l` (modo de escuta)
  - `nc -p` (especifica uma porta)
  - `nc -u` (usa o protocolo UDP em vez de TCP)
  - `nc -z` (modo de escaneamento de porta sem enviar dados)
  - `nc -v` (modo verbose, exibe mais detalhes)

- **Exemplos de uso:**
  - `nc -l -p 1234` (escuta na porta 1234)
  - `nc -v google.com 80` (conecta ao Google na porta 80 com detalhes)
  - `nc -u -l -p 1234` (escuta na porta 1234 usando UDP)
  - `nc -zv 192.168.1.1 80` (faz varredura de portas para o IP 192.168.1.1 na porta 80)
  - `nc -zv 192.168.1.1 1-1000` (escaneia as portas de 1 a 1000 no IP 192.168.1.1)

---

## 13. `telnet`
**Significado:** Protocolo de rede para comunicação com outros dispositivos.

**Sintaxe**
`telnet [hostname] [port]`

- **Exemplos de uso:**
  - `telnet google.com 80` (conecta ao Google na porta 80)
  - `telnet localhost 23` (conecta ao serviço Telnet na máquina local, porta padrão 23)
  - `telnet 192.168.1.1` (conecta ao IP 192.168.1.1 na porta padrão do Telnet)
  
  **Observação:** O Telnet é uma ferramenta antiga e insegura para muitas situações modernas, onde o SSH é recomendado.

---

## 14. `find`
**Significado:** Localizar arquivos e diretórios no sistema.

**Sintaxe**
`find [caminho] [opções] [expressão]`

- **Opções:**
  - `find -name` (procura por arquivos com nome específico)
  - `find -type` (filtra por tipo de arquivo: `f` para arquivo, `d` para diretório)
  - `find -size` (procura por arquivos com um tamanho específico)
  - `find -exec` (executa um comando em cada arquivo encontrado)
  - `find -mtime` (procura arquivos modificados dentro de um período de tempo)
  - `find -user` (procura arquivos pertencentes a um determinado usuário)
  - `find -perm` (procura arquivos com permissões específicas)

- **Exemplos de uso:**
  - `find /home/usuario -name "*.txt"` (encontra todos os arquivos .txt no diretório do usuário)
  - `find / -type f -size +10M` (encontra arquivos maiores que 10 MB em todo o sistema)
  - `find /var/log -mtime -7` (encontra arquivos modificados nos últimos 7 dias no diretório /var/log)
  - `find /home/usuario -name "*.jpg" -exec rm {} \;` (encontra e apaga todos os arquivos .jpg no diretório do usuário)
  - `find / -user root` (encontra todos os arquivos pertencentes ao usuário root)
  - `find / -perm 755` (encontra arquivos com permissões 755)
  
---

## 15. `chmod` (Change Mode)
**Significado:** Alterar permissões de arquivos ou diretórios.

**Sintaxe**
`chmod [modo] [arquivo]`

**Representação das permissões:**
As permissões podem ser definidas de duas maneiras: simbólica e numérica.

1. Notação simbólica:
    - As permissões são representadas por letras:
        `r`: Permissão de leitura (read).
        `w`: Permissão de escrita (write).
        `x`: Permissão de execução (execute).
    
    - As permissões são atribuídas a três grupos:
        `u`: Proprietário do arquivo (user).
        `g`: Grupo do arquivo (group).
        `o`: Outros usuários (others).
        `a`: Todos (all).

2. Notação numérica:
    - As permissões são representadas por números, onde cada permissão tem um valor:
        `4`: Leitura (r).
        `2`: Escrita (w).
        `1`: Execução (x).
    - As permissões são somadas para cada grupo:
        `7`: Leitura, escrita e execução (4+2+1).
        `6`: Leitura e escrita (4+2).
        `5`: Leitura e execução (4+1).
        `4`: Leitura.
        `3`: Escrita e execução (2+1).
        `2`: Escrita.
        `1`: Execução.
        `0`: Sem permissões.

- **Opções:**
  - `chmod +x` (adiciona permissão de execução)
  - `chmod -r` (remove permissão de leitura)
  - `chmod u+r` (adiciona permissão de leitura ao proprietário)
  - `chmod g+w` (adiciona permissão de escrita ao grupo)
  - `chmod o+x` (adiciona permissão de execução para outros)
  - `chmod 755` (define permissões numéricas)

- **Exemplos de uso:**
  - `chmod +x script.sh` (adiciona permissão de execução ao arquivo script.sh)
  - `chmod u+r arquivo.txt` (dá ao proprietário permissão de leitura no arquivo.txt)
  - `chmod g+w arquivo.txt` (dá ao grupo permissão de escrita no arquivo.txt)
  - `chmod 755 arquivo.sh` (define permissões de leitura, escrita e execução para o dono e leitura e execução para o grupo e outros)

---

## 16. `chown` (Change Ownership)
**Significado:** Alterar proprietário e/ou o grupo de arquivos ou diretórios.

**Sintaxe**
`chown novo_proprietario[:novo_grupo] arquivo`

- **Opções:**
  - `chown user` (muda o proprietário do arquivo)
  - `chown user:group` (muda o proprietário e o grupo)
  - `chown -R` (altera o proprietário recursivamente)
  
- **Exemplos de uso:**
  - `chown usuario arquivo.txt` (muda o proprietário de arquivo.txt para "usuario")
  - `chown usuario:grupo arquivo.txt` (muda o proprietário e o grupo de arquivo.txt)
  - `chown -R usuario /home/usuario/pasta` (altera o proprietário de todos os arquivos dentro de "pasta" para "usuario")

---

## 17. `df` (Disk Free)
**Significado:** Exibir o uso de espaço em disco.

**Sintaxe**
`df [opções]`

- **Opções:**
  - `df -h` (exibe o uso de disco em formato legível)
  - `df -T` (exibe o tipo de sistema de arquivos)
  - `df -i` (mostra o uso de inodes)
  
- **Exemplos de uso:**
  - `df` (exibe o uso de espaço em disco)
  - `df -h` (exibe o uso de disco com unidades legíveis, como GB e MB)
  - `df -T` (mostra o tipo de sistema de arquivos para cada partição)
  - `df -i` (exibe a quantidade de inodes usados)
  - `df /caminho/para/diretorio` (exibe )

---

## 18. `du` (Disk Usage)
**Significado:** Exibir o uso de espaço em disco por arquivos e diretórios.

**Sintaxe**
`du [opções] [caminho]`

- **Opções:**
  - `du -h` (exibe o uso de disco em formato legível)
  - `du -s` (mostra o total do diretório especificado)
  - `du -c` (mostra um total cumulativo)

- **Exemplos de uso:**
  - `du` (mostra o uso de disco por arquivos e diretórios no diretório atual)
  - `du -h` (mostra o uso de disco em um formato legível)
  - `du -s /home/usuario` (mostra o uso total de disco em /home/usuario)
  - `du -c /home/usuario/*` (mostra o uso de disco para todos os arquivos/diretórios em /home/usuario com um total cumulativo)

---

## 19. `ps` (Process Status)
**Significado:** Exibir informações sobre processos em execução.

**Sintaxe**
`ps [opções]`

- **Opções:**
  - `ps -e` (exibe todos os processos)
  - `ps -f` (exibe uma lista completa com mais detalhes)
  - `ps -u <usuário>` (filtra processos por usuário)
  - `ps -aux` (exibe todos os processos com detalhes)
  - `ps -e --forest` (exibe os processos em uma estrutura de árvore, mostrando a hierarquia entre eles)
  - `ps -a` (exibe processos de todos os usuários)
  - `ps -x` (exibe processos que não têm um terminal associado (processos em segundo plano))
  
- **Exemplos de uso:**
  - `ps` (exibe os processos do usuário atual no terminal)
  - `ps -e` (lista todos os processos em execução)
  - `ps -f` (exibe processos com mais detalhes, como PID, tempo, etc.)
  - `ps -u root` (lista processos que pertencem ao usuário root)
  - `ps -aux` (mostra todos os processos detalhados)

---

## 20. `kill`
**Significado:** Enviar sinais para encerrar processos.

**Sintaxe**
`kill [opções] <PID>`

- **Opções:**
  - `kill -9` (força o encerramento do processo)
  - `kill -l` (lista todos os sinais disponíveis)

- **Exemplos de uso:**
  - `kill 1234` (envia o sinal de término para o processo com PID 1234)
  - `kill -9 1234` (força o encerramento do processo 1234)
  - `kill -l` (exibe a lista de sinais que podem ser enviados para processos)

---

## 21. `mkdir` (Make Directory)
**Significado:** Criar diretórios.

**Sintaxe**
`mkdir [opções] <nome_do_diretorio>`

- **Opções:**
  - `mkdir -p` (cria diretórios pai se eles não existirem)
  - `mkdir -v` (exibe uma mensagem para cada diretório criado)
  - `mkdir -m` (define as permissões do diretório a ser criado)

- **Exemplos de uso:**
  - `mkdir pasta` (cria um diretório chamado "pasta")
  - `mkdir -p /home/usuario/pasta/subpasta` (cria subdiretórios no caminho especificado, se necessário)
  - `mkdir -v pasta` (mostra uma mensagem ao criar "pasta")
  - `mkdir -m 755 novo_diretorio` (cria um diretório com permissões específicas)

---

## 22. `rmdir` (Remove Directory)
**Significado:** Remover diretórios vazios.

**Sintaxe**
`rmdir nome_do_diretorio`

- **Opções:**
  - `rmdir -p` (remove um diretório e seus pais, se estiverem vazios)

- **Exemplos de uso:**
  - `rmdir pasta` (remove o diretório "pasta" se estiver vazio)
  - `rmdir -p /home/usuario/pasta` (remove "pasta" e diretórios pais se todos estiverem vazios)

---

## 23. `rm` (Remove)
**Significado:** Remover arquivos ou diretórios.

**Sintaxe**
`rm [opções] <nome_do_arquivo_ou_diretorio>`

- **Opções:**
  - `rm -r` (remove diretórios e seus conteúdos recursivamente)
  - `rm -f` (força a remoção sem pedir confirmação)
  - `rm -i` (pede confirmação antes de remover cada arquivo)

- **Exemplos de uso:**
  - `rm arquivo.txt` (remove arquivo.txt)
  - `rm -r pasta` (remove "pasta" e todos os arquivos/diretórios contidos nela)
  - `rm -f arquivo.txt` (remove forçadamente sem pedir confirmação)
  - `rm -i arquivo.txt` (pede confirmação antes de remover)

---

## 24. `history`
**Significado:** Exibir o histórico de comandos digitados no terminal.

- **Opções:**
  - `history -c` (limpa o histórico)
  - `history <número>` (exibe os últimos "número" comandos)
  - `history -d <número>` (remove o comando do histórico especificado pelo número)
  - `history -a` (salva o histórico atual no arquivo de histórico)
  - `history -r` (lê o histórico do arquivo de histórico e o adiciona à sessão atual)

- **Exemplos de uso:**
  - `history` (mostra o histórico de comandos)
  - `history 20` (mostra os últimos 20 comandos)
  - `history -c` (limpa o histórico de comandos)

---