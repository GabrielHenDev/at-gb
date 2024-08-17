##REQUESITOS 

-UBUNTU 20.04 (OBRIGATORIO)
-VM COM MINIMO: 2CPU 4GB RAM
-VM COM RECOMENDADO: 4CPU 6GB RAM


## CRIAR SUBDOMINIO E APONTAR PARA O IP DA SUA VPS ##

FRONTEND_URL: app.seudominio.com
BACKEND_URL:  api.seudominio.com

## CHECAR PROPAGAÇÃO DO DOMÍNIO ##

https://dnschecker.org/

## COPIAR A PASTA PARA ROOT E RODAR OS COMANDOS ABAIXO no Seu SERVIDOR SSH ##

cd ./whaticket
sudo chmod +x whaticketsaas
sudo ./whaticketsaas

===================================================

login: admin@admin.com
senha: 123456

===================================================

Configuração de e-mail dentro do BACKEND no arquivo ENV

MAIL_HOST="smtp.gmail.com"
MAIL_USER="seu-email"
MAIL_PASS="sua-senha"
MAIL_FROM="seu-email"
MAIL_PORT="587"

Configuração de pagamento GERENCIANET dentro BACKEND no arquivo ENV

GERENCIANET_SANDBOX=true
GERENCIANET_CLIENT_ID=sua-id
GERENCIANET_CLIENT_SECRET=sua_chave_secreta
GERENCIANET_PIX_CERT=nome_do_certificado
GERENCIANET_PIX_KEY=chave_pix_gerencianet

# para usar GERENCIANET Em backend\certs
# Salvar o certificado no formato .p12




Preparação para instalação...
------
-
Para a instalação você vai precisar:

- Recomendações -

Sistema------------------

⚠️Ubuntu 20.04

Nosso token de Acesso, vai pedir para instalação...


-----

( Vai precisar de 2 subdomínio )

Subdomínio para Frontend 👉🏻 https://app.nomedoseudominio.com
Subdomínio para API (Backend) 👉🏻 https://api.nomedoseudominio.com

Frontend - app.nomedoseudominio.com
Backend - api.nomedoseudominio.com


## COPIAR A PASTA PARA ROOT E RODAR OS COMANDOS ABAIXO ##

-----

sudo apt update && sudo apt install -y git && git clone https://github.com/.../instalador.io.git && cd instalador.io && chmod +x panel.sh && ./panel.sh

-----
