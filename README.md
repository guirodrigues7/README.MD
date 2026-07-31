# *Introdução ao Back End*

## **Back-End**
* Back-End é o que os usuários não veem. Considerado 80% do esforço total. (Enquanto o front seriam os outros 20%). Ele é quem gerencia os dados invisiveis, onde as regras do sistema realmente vivem, lida com a conexão entre diferentes sistemas, garantindo que tudo funcione nos bastidores, o usuário não consegue ver ou interagir diretamente.
    * Obs: quando você da o comando f12, não consegue ver o código.
        * *Exemplo do restaurante:* O cliente geralmente é o (front) quem deseja fazer um pedido. O garçom (API) anota e leva o pedido sem expor os segredos da cozinha. A resposta seria a cozinha (back-end) processa a socilitação e entrega a refeição.

## **API**
* Uma API é a ponte essencial e invisível que conecta a interface gráfica (Front-end) à inteligência e ao armazenamento do sistema (Back-end e Banco de Dados). Ela permite que o usuário solicite ações e receba dados sem nunca expor a estrutura interna da aplicação. 

* Para ser considerada de alto nível, uma API deve cumprir três pilares:
*Organizada:* Possui rotas claras, semânticas e previsíveis (ex: GET /produtos, POST /pedidos).
*Limpa:* Devolve apenas o necessário para a tela, sem "sujeira" ou campos inúteis no payload.
*Rápida:* Processa requisições em milissegundos, utilizando rotas otimizadas e cache inteligente.

## *Para que Serve uma API?*

#### *Objetivo principal:* Garantir que diferentes sistemas conversem de forma segura, padronizada e eficiente.
#### *Desacoplamento:* Separa a lógica do Back-end da interface do Front-end. Isso permite que você mude o visual do site sem precisar reescrever as regras do banco de dados (e vice-versa).
#### *Segurança e Escudo de Dados:* O banco de dados nunca fica exposto diretamente à internet. A API valida a autenticação, autoriza permissões e filtra tudo o que entra e sai.
#### *Reutilização de Código (Omnichannel):* A mesma API pode alimentar o site web, o aplicativo Android, o app do iPhone e até relógios inteligentes simultaneamente.
#### *Integração de Ecossistemas:* Permite que sistemas de empresas diferentes se conectem (como seu aplicativo usando a API do Pix, do Google Maps ou de um gateway de pagamento).

# **NODE.JS**
* O criador foi Ryan Dahl em 2009
A tecnologia é baseado no poderoso motor v8 do Google.
Permite executar codigo Java Script do lado do servidor (BACK END)

   #### *NPM:* Node Package Manager (Gerenciador de Pacotes do Node);
   #### *NPX:* Node Package Execute (Executor de Pacotes do Node) 

# ~~COMANDOS~~
* #### *CHALK-* O Chalk é uma biblioteca do Node.js usada para colorir e estilizar textos 
    * Install: npm install chalk;
               /npx chalk
        * *Exemplos:* 
import chalk from 'chalk';
console.log(chalk.blue('Hello world!'));

* #### *FIGLET-* O comando figlet transforma textos comuns em letras grandes feitas com arte ASCII direto no terminal do Linux ou macOS. Ele serve para criar banners chamativos, enfeitar scripts ou personalizar mensagens de boas-vindas.
    * Install: npm install figlet
               /npx figlet
        * *Exemplos:* 
import figlet from "figlet";

async function doStuff() {
  const text = await figlet.text("Hello World!!");
  console.log(text);
}

doStuff();

* #### *NODEMON-* O nodemon reinicia seu servidor Node.js automaticamente toda vez que você altera e salva um arquivo no código. Ele poupa o trabalho de fechar e abrir o programa no terminal a cada mudança, acelerando bastante a criação de sites e sistemas.
    * Install: npm install -g nodemon
            /npx nodemon
