# Estrutura de Diretórios no Linux

## 1. Diretório `/bin`

O diretório `/bin` contém executáveis essenciais do sistema, que são programas utilizados para tarefas básicas, como o `bash`, `cat`, `ls` e `firefox`. Além dos executáveis, também podemos encontrar links simbólicos e scripts de shell, que são sequências de comandos que podem ser executadas. Este diretório é semelhante à pasta “C:\Program Files” no Windows, mas aqui os arquivos estão organizados em ordem alfabética e não por fabricante.

## 2. Diretório `/boot`

O diretório `/boot` é crucial para o funcionamento do sistema, pois armazena os arquivos necessários para a inicialização do computador. Isso inclui o bootloader (como o GRUB) e as entradas do Kernel. Recomenda-se não fazer alterações nesse diretório a menos que o usuário tenha conhecimento técnico.

## 3. Diretório `/dev`

A pasta `/dev` é a representação de dispositivos de hardware no Linux. Cada dispositivo conectado ao seu computador (como HDs e SSDs) é tratado como um arquivo. Os arquivos dentro deste diretório permitem a configuração e o controle dos dispositivos. Por exemplo, as unidades são referenciadas como `/dev/sda` ou `/dev/sdb`.

## 4. Diretório `/etc`

O diretório `/etc` armazena arquivos de configuração que se aplicam a todo o sistema, ou seja, são configurações “system-wide”. Isso inclui configurações de rede, serviços e outros aspectos do sistema. As configurações específicas de usuários são armazenadas em outro diretório.

## 5. Diretório `/home`

A pasta `/home` é onde ficam os diretórios dos usuários comuns do sistema. Dentro desse diretório, são encontradas as subpastas nomeadas com os nomes dos usuários cadastrados. Aqui, cada usuário tem seu próprio espaço, incluindo pastas para documentos, imagens e configurações pessoais. É importante notar que esta pasta contém arquivos ocultos que guardam preferências e configurações de aplicativos.

## 6. Diretórios `/lib`, `/lib32`, `/lib64`, `/libx32`

Esses diretórios contêm bibliotecas de software essenciais para o funcionamento do sistema e de programas instalados. O diretório `/lib` é destinado a bibliotecas de arquitetura múltipla, enquanto `/lib32` e `/lib64` são específicos para bibliotecas de 32 e 64 bits, respectivamente. O diretório `/libx32` é menos comum, mas é utilizado para bibliotecas específicas com ABI x32.

## 7. Diretório `/media`

O diretório `/media` é o local onde as unidades removíveis, como pen drives e HDs externos, são montadas automaticamente pelo sistema. Quando um dispositivo é conectado, seu conteúdo pode ser acessado diretamente nesse diretório.

## 8. Diretório `/mnt`

O diretório `/mnt` é utilizado como um ponto de montagem para unidades de disco que os usuários montam manualmente. Embora seja possível montar unidades onde quisermos, esse diretório serve como uma sugestão amigável para facilitar a organização.

## 9. Diretório `/opt`

A pasta `/opt` é destinada a softwares instalados por fabricantes ou softwares proprietários. Aqui, são encontradas aplicações que não fazem parte da instalação padrão do sistema, permitindo uma organização clara.

## 10. Diretório `/proc`

O diretório `/proc` é um diretório virtual que fornece informações sobre o sistema e seus processos. Ele não armazena arquivos no disco, mas gera arquivos a cada inicialização. Cada processo em execução possui um diretório correspondente, permitindo monitorar e gerenciar os processos ativos.

## 11. Diretório `/root`

O diretório `/root` é o espaço pessoal do usuário Root, similar ao `/home`, mas com permissões especiais. Este diretório é separado para garantir que o usuário Root tenha um ambiente seguro e isolado para realizar tarefas administrativas.

## 12. Diretório `/run`

O diretório `/run` é um diretório virtual que é criado na memória durante a inicialização do sistema. Ele armazena informações temporárias sobre o estado do sistema, como usuários logados e serviços em execução. Esses dados são perdidos quando o sistema é desligado.

## 13. Diretório `/sbin`

Semelhante ao `/bin`, o diretório `/sbin` contém binários de sistema, mas são programas acessíveis apenas ao administrador. Aqui estão comandos críticos que requerem privilégios elevados para execução, como o comando `useradd`.

## 14. Diretório `/snap`

O diretório `/snap` é usado para armazenar pacotes Snap, um formato de empacotamento desenvolvido pela Canonical. O suporte a pacotes Snap é comum em distribuições baseadas no Ubuntu.

## 15. Diretório `/srv`

A pasta `/srv` é destinada ao armazenamento de arquivos de serviços que serão acessíveis para outros usuários. Essa estrutura facilita a administração e a segurança, permitindo que os arquivos sejam montados a partir de discos separados.

## 16. Diretório `/sys`

O diretório `/sys` é um meio de interagir com o Kernel Linux. Ele contém informações sobre dispositivos e drivers. Assim como o `/run`, não armazena arquivos no disco, mas é gerado a cada inicialização.

## 17. Diretório `/tmp`

O diretório `/tmp` é utilizado para armazenar arquivos temporários que os programas podem precisar durante uma sessão. Os arquivos aqui devem ser excluídos após a reinicialização do sistema. Algumas distribuições utilizam um sistema de arquivos virtual chamado `tmpfs` para gerenciar essa pasta.

## 18. Diretório `/usr`

O diretório `/usr` é onde são encontrados arquivos de programas e bibliotecas que são úteis para os usuários, mas não essenciais para o funcionamento básico do sistema. Este diretório também contém o subdiretório `local`, que é onde as aplicações instaladas a partir de código fonte são frequentemente armazenadas.

## 19. Diretório `/var`

Finalmente, o diretório `/var` armazena arquivos que se espera que aumentem de tamanho, como logs, cache e arquivos de backup. É importante diferenciar o cache do sistema, que fica aqui, do cache do usuário, que é armazenado na pasta oculta `.cache` dentro do diretório `/home` de cada usuário.

---