Esta api servira para ler um arquivo json com dados do cadsus, 
tratar os dados e inserir no banco de dados MySQL

A extrutura para criar as colunas do banco de dados sera a seguinte:

     Dados Pessoais 
     CNS 
     Nome: ,  Nome Social / Apelido 
     Nome da Mãe: ,  Nome do Pai 
     Sexo: ,  Raça 
     Data de Nascimento: ,  Tipo Sanguíneo 
     Nacionalidade: ,  Município de Nascimento 
     Endereço 
     Tipo Logradouro: ,  Logradouro 
     Complemento: ,  Número 
     Bairro: ,  CEP 
     País de Residência: ,  Município de Residência 
     Contatos 
     Telefone 
     Documentos 
     CPF 
     Identidade:


   


# SCRAPING CADSUS v1.0

### Atualizaçoes

O Codigo esta em costante atualização!

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

* Você instalou a versão mais recente do `NodeJS`
* Você tem uma máquina `<Windows / Linux / Mac>`.
* Você tem um `Login` de Operador do sistema `CADSUSiii`.

## 💻 Oque essa API Faz

O projeto ainda está em desenvolvimento e atualizaçoes estao sendo feitas constantemente:

Este código é um script de raspagem de dados que utiliza o framework Puppeteer para automatizar a navegação em um site específico, neste caso, é o CADSUSiii.saude.gov.br. Ele também utiliza outras bibliotecas como o readline, stealthplugin, fs, figlet, chalk e open para realizar tarefas adicionais, como lidar com o console, capturar imagens, lidar com captchas e abrir arquivos. O objetivo deste script é automatizar o processo de login e coleta de informações do site, como dados de pacientes. Ele foi feito por Dixavado e pode ser contatado pelo número 61 9235-5359.


## 🚀 Exemplo de Resultado Salvo

```
 [
            "700703906787174 "
        ],
        [
            "MARGARETE AMARO ANTIQUEIRA",
            "---"
        ],
        [
            "MARIA DO CARMO DA CONCEICAO AMARO",
            "MARCOS ANTONIO FRAGA DO AMARAL ANTIQUEIRA"
        ],
        [
            "FEMININO",
            "PRETA"
        ],
        [
            "14/08/1983 (39 anos)",
            "---"
        ],
        [
            "BRASILEIRA",
            "RIO GRANDE - RS"
          ],
        [
            "INVALIDO",
            "HONORIO BICALHO"
        ],
        [
            "---",
            "11"
        ],
        [
            "GETULIO VARGAS",
            "---"
        ],
        [
            "BRASIL",
            "RIO GRANDE - RS"
          ],
        [
            " Tipo Telefone  tDDD  tNúmero OUTRO  t(21)  t2105-0000     ",
            "Tipo Telefone",
            "(21)",
            "2105-0000"
         ],
        [
            " 025.680.090-12"
        ],

```

## ☕ Usando o Script 

Para usar CADSUS Scraping, primeiro adiquira uma `licença` para rodar o Script `CADSUS Scraping`.
Configure o arquivo `.env` com o `Nome de Usuario e Senha` de `Operador do CADSUS`.
Rode o Script `Validador de CPF` para validar sua `DB` de `CPF`, para evitar erros de `CPF Invalido`
Rode o Script `CADSUS Scraping`.
    ( Certifique-se de que os CPF estao no arquivo lista.txt)
Apos iniciar o `Script`, sera exibida as seguintes menssagens na Tela:
    - ⌛ Aguarde a imagem do Captcha ser Iniciado ⌛
      ( `Script` aguardando a geração do `ReCaptcha` do Site )
    - 🤳 Captcha Carregado com Sucesso! 🤳
      ( O `Script` salva uma imagem contendo o Texto do `ReCaptcha` e abre o arquivo para o usuario)
    - 🖥️ Digite o codigo do Captcha e aperte Enter
      ( Digite o `Valor` do `ReCaptcha` de acordo com a `Imagem do ReCaptcha` que foi aberta )
    - 🔑 Logado com Sucesso
      ( O `Script` fez login com Sucesso no Site do `CADSUS`)
    - 🗒️ CPF Carregados:
      ( Exibe a `quantidade` de `CPF` carregados )


                            ❗❕ ATENÇÃO: ❕❗
                SE FOR GERADO QUALQUER TIPO DE ERRO APOS O LOGIN
                   SIGNIFICA QUE OUVE ALGUM PROBLEMA NO LOGIN
                   REINICIE O SCRIPT E FAÇA O LOGIN NOVAMENTE

    
      
## ☕ Como Iniciar o Script 

Abra o `Terminal` como `Administrador` e acesse a pasta que contem o arquivo `app.js` 
Exemplo:
```
cd C://CADSUS-Scraping
```

Apos isso de os Seguintes Comandos:
```
npm i
node app.js
```

Comando: npm i ( Instala as dependencias do Script )
Comando: node app.js ( Inicia o Script )
