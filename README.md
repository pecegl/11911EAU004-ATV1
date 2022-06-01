# Aluno: Pedro Cunha Garcia Lopes - 11911EAU004

## Atividade 1 Sistemas Embarcados

### Etapas

Primeiramente foi feita a ativação da virtualização da máquina através do sistema e da BIOS. Essa etapa foi necessária para a instalação do Ubuntu 20.04 através do Windows PowerShell. Foi criado usuário e senha, feitas as atualizações e criação do ambiente de trabalho com a criação dos diretórios.
Em seguida, fiz a instalação do compilador GCC - GNU C Compiler e a ferramenta de controle de versões Git. Além disso, também instalei o GCC ARM Toolchain, o OpenOCD, ST-LINK Tools e do IDE Visual Studio Code e suas extensões. Finalizando as preparações de ambiente, instalei o USBIP e configurei a conexão do gravador ST-LINK.\
Começando a etapa de códigos, começamos por criar o primeiro arquivo main.c para que pudesse compreender o funcionamento do compilador. Posteriormente, foi inserido o arquivo Makefile. Foi criada uma regra para a compilação do main.c e em seguida uma para remover os arquivos objetos gerados na compilação.\
Neste momento foi criado o arquivo de inicialização com o nome startup.c, nesse arquivo declaramos e inicializamos o Stack e a Tabela de Vetores de Interrupção além de fazer o código do Reset handler e de exception handler.

### Detalhamento dos Arquivos

#### main.c

#### Makefile

O make é utilizado para automatizar o processo de compilação utilizando instruções contidas em arquivos chamados Makefile. Neste arquivo, teremos as instruções de compilação dos outros arquivos do projeto para que sejam gerados os arquivos de formato .o, .elf e .bin. As instruções ccontêm 5 tipos de elementos: regras explicitas, regras implicitas, definições de variáveis, diretivas e comentários. A regra informa ao make quando um traget está destualizado e como fazer para atualizá-lo. Seu formato é: <br>targets: prerequisites. <br>recipe.

#### startup.c

O startup. é o arquivo de incialização

#### stm32f411-rom.ld

