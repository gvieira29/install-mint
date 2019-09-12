# GUIA DE INSTALAÇÃO – LINUX MINT 19.2 “TINA”

O Linux Mint é uma distribuição muito popular baseado no Ubuntu, e uma das mais conhecidas entre os iniciantes do mundo Linux por ser fácil o uso, e por sua aparência semelhante ao da *Microsoft*.  

Este guia ira mostrar como instalar o Linux Mint 19.2 com a interface Cinnamon, mas o método utilizado aqui, é o mesmo em outras versões e interfaces, pois o instalador não muda.
Antes de instalar, verifique as configurações da maquiná que deseja instalar, é recomendável ter um mínimo de 2GB de RAM e também 15GB de espaço livre no HD.  

## SESSÃO LIVE

Ao dar *boot* pela primeira vez você ira ver esta tela abaixo, aqui já é possível você utilizar e testar o sistema, antes de iniciar a instalação, o sistema esta rodando diretamente do pendrive e assim você pode verificar na sua máquina se realmente agradou e deseja prosseguir a instalação.  
[IMAGEM]

## INSTALAÇÃO

Antes de iniciar, é recomendável que a maquina esteja conectada na internet para durante a instalação o sistema poder baixar alguns pacotes da rede.  

Se você não possui a imagem de instalação, pode baixar diretamente do site Linux Mint, clicando [aqui](https://www.linuxmint.com/download.php), você será redirecionado a página de downloads.  

- PASSO 1: Abra o menu de instalação, clicando no ícone de um CD **“Install Linux Mint”**.  
[IMAGEM]

- PASSO 2: Selecione o idioma que deseja utilizar no sistema, aqui vamos usar Português do Brasil.  
[IMAGEM]

- PASSO 3: Selecione qual o tipo de teclado, se você não souber qual teclado é o seu, basta utilizar a detecção automática de layout.  
[IMAGEM]

- PASSO 4: Selecione se deseja ou não instalar software de terceiros. (Se esta acostumado com Windows, marque esta opção, para instalação de drivers para gráfico, Wi-Fi, flash, MP3 e outros).  
[IMAGEM]

- PASSO 5: Aqui vocẽ pode escolher como instalar o sistema, e configurar o particionamento. No nosso caso vamos “Apagar o disco e Instalar o Linux Mint”.  
(Se você estiver instalando em Dual-Boot, devera instalar o Linux Mint ao lado do seu sistema operacional, e determinar quanto do disco você deseja usar.)  
[IMAGEM]

- PASSO 6: Confirme as alterações a serem feitas e prossiga.  
[IMAGEM]

- PASSO 7: Selecione a região para definir seu fuso horário.  
[IMAGEM]

- PASSO 8: Dar um nome a sua maquina e criar seu Usuário e Senha.  
[IMAGEM]

*Um exemplo de como deverá ser preenchido*  
[IMAGEM]

- PASSO 9: Agora basta esperar que a instalação seja feita, este processo poderá levar alguns minutos, dependendo da configuração da sua maquina.  
[IMAGEM]

- PASSO 10: Após a instalação acabar, basta reiniciar a maquina.  
[IMAGEM]

Não se esqueça de remover a mídia de instalação antes de reiniciar a maquina, remova e tecle Enter  
[IMAGEM]

Pronto o Sistema operacional esta instalado e pronto para ser usado.  
[IMAGEM]

## ATUALIZAÇÃO DO SISTEMA

Com o nosso sistema instalado, você pode fazer uma atualização, vamos fazer um guia rápido, acompanhe:  

- PASSO 1: Vamos definir uma senha de Administrador do sistema (root), ou Super Usuário. Abra um terminal e digite:  
```bash
sudo passwd
```
[IMAGEM]

Ira pedir para digitar sua senha, a do seu usuário, em seguida uma nova senha de administrador, e então uma confirmação. Apos ter confirmado a senha você deverá estar nessa tela.  
[IMAGEM]

- PASSO 2: Digite o comando su, ira pedir a senha de Administrador que você acabou de criar.  
```bash
su
```
[IMAGEM]

- PASSO 3: Por ultimo, basta rodar o comando abaixo que ira atualizar o seu sistema, não é necessário reiniciar, mas é recomendável uma reinicialização após atualizar, para aplicar as mudanças.  
```bash
apt-get update && apt-get upgrade -y
```
[IMAGEM]

`apt-get update` == atualiza o repositório, verificando por novas atualizações.  
`apt-get upgrade` == faz baixa e instala as atualizações, o termo `-y` na frente, representa yes, se não for utilizado, quando rodar o comando, ira perguntar se você deseja realmente instalar as atualizações, dando as opções `[Y/N]`, deixando tudo junto, rodamos apenas um comando, deixando o dia a dia mais prático.