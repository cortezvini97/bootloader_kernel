# Bootloader And Kernel

Aqui estão os comandos para compilar código Assembly usando o NASM (Netwide Assembler).

## Compilando o bootloader

Para compilar um arquivo de código Assembly chamado `bootloader.asm` em um arquivo binário chamado `bootloader.bin`, você pode usar o seguinte comando:

```shell
nasm -f bin bootloader.asm -o bootloader.bin
````

## Compilando o kernel

Para compilar um arquivo de código Assembly chamado `kernel.asm` em um arquivo binário chamado `kernel.bin`, você pode usar o seguinte comando:

```shell
nasm -f bin kernel.asm -o kernel.bin
````

## Montando a imagem e gravando em um pendrive

Após compilar seus arquivos Assembly, você pode montar a imagem resultante em um pendrive usando o programa FergoRaw e gravá-la no dispositivo com o Rufus. Aqui estão os passos para fazer isso:

Montando a imagem com o FergoRaw:

Abra o programa FergoRaw.
Clique em "File" ou "Arquivo" no menu e selecione "Open" ou "Abrir".
Navegue até o local onde você salvou o arquivo binário (por exemplo, bootloader.bin) e abra-o no FergoRaw.
Certifique-se de selecionar o dispositivo USB ou a unidade que deseja usar para criar a imagem.
Gravando a imagem com o Rufus:

Baixe e execute o Rufus em seu sistema.
Selecione o dispositivo USB que você deseja usar para criar o pendrive inicializável.
Clique em "Select" ou "Selecionar" ao lado de "Boot selection" ou "Seleção de Inicialização" e escolha o arquivo binário (por exemplo, kernel.bin) que você compilou.
Configure as opções de formatação e rótulo do pendrive conforme necessário.
Clique em "Start" ou "Iniciar" para iniciar o processo de criação do pendrive inicializável.
Agora você terá um pendrive inicializável com sua imagem Assembly compilada, pronto para ser usado em seu projeto ou sistema.

Lembre-se de consultar a documentação e os manuais de uso do FergoRaw e do Rufus para obter informações adicionais sobre o uso dessas ferramentas.