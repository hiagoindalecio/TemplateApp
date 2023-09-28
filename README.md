
# Tutorial básico React Native
Este é um tutorial exemplificado de como inicializar o desenvolvimento de uma aplicação mobile utilizando o [React Native](https://reactnative.dev), o [typescript](https://www.typescriptlang.org) e o [yarn](https://yarnpkg.com) como gerenciador de pacotes.

# Introdução 
Primeiramente, é necessária um breve introdução das ferramentas que serão utilizadas durante o desenrolar do tutorial, para o bom entendimento do processo e facilitação do aperfeiçoamento dos conhecimentos que serão  obtidos aqui.

## Node.js
O [Node.js](https://nodejs.org/pt-br) é um *runtime* JavaScript desenvolvido com o [Chrome's V8 JavaScript engine](https://v8.dev/), que basicamente serve para executar códigos JavaScript fora de um navegador web de forma assíncrona, tendo sua arquitetura orientada por eventos.

## VisualStudio Code
O [VisualStudio Code](https://code.visualstudio.com) é um poderoso editor de código fonte que vem com suporte integrado para JavaScript, TypeScript e Node.js, além de um rico ecosistema de extensões das mais variadas.

## React Native
O [React Native](https://reactnative.dev) é uma biblioteca JavaScript criada pelo Facebook, usada para desenvolver aplicativos móveis para os sistemas Android e iOS de forma nativa, não havendo a necessidade do desenvolvimento dedicado à um sistema operacional específico, já que o código JavaScript é renderizado como código nativo pela biblioteca.

## Yarn
O [Yarn](https://yarnpkg.com), criado pelo Facebook, é um estável gerenciador de pacotes análogo ao [npm](https://www.npmjs.com), gerenciador de pacotes padrão do [Node.js](https://nodejs.org/pt-br). O [Yarn](https://yarnpkg.com) é utilizado no gerenciamento de dependências de projetos JavaScript e dá assistência à instalação, atualização, configuração e remoção de pacotes, sendo considerado mais rápido e seguro que o [npm](https://www.npmjs.com) pela comunidade de desenvolvedores que utilizam a tecnologia.

## Typescript
O [Typescript](https://www.typescriptlang.org) é basicamente JavaScript, porém com sintaxe para torna-lo fortemente tipado. O [Typescript](https://www.typescriptlang.org) é altamente recomendado à desenvolvedores JavaScript iniciantes, pois permite uma melhor percepção do código em tempo de desenvolvimento e evita a ocorrência de erros na utilização de ferramentas por conta da tipagem.

## npx
O [npx](https://docs.npmjs.com/cli/v7/commands/npx) (Node Package eXecute) é um executante de pacotes node locais ou remotos.

## Expo Go
O [Expo Go](https://expo.dev/client) serve para rodar aplicações em servidores de desenvolvimento em dispositivos móveis através da rede de forma rápida.
[Post recomendado](https://blog.rocketseat.com.br/expo-react-native/)

# Passo-a-passo
 **1. Instalação do Node.js**
 <br />
Antes de qualquer coisa, será necessário realizar a instalação do Node.js na máquina. O arquivo instalador pode ser obtido diretamente no [site oficial](https://nodejs.org/pt-br) da ferramenta.
<br />
![Botão de instalação do Node.js no site oficial](https://github.com/hiagoindalecio/TemplateApp/blob/main/Node.png?raw=true)
<br />
Recomento a instalação da versão recomendada para evitar a ocorrência de erros.

**2. Instalação do VisualStudio Code**
<br />
É possível a instalação através do [site oficial](https://code.visualstudio.com) da ferramenta, o botão de instalação virá pré-definido de acordo com seu sistema operacional:
<br />
![Botão de instalação do VisualStudio Code no site oficial](https://github.com/hiagoindalecio/TemplateApp/blob/main/VsCode.png?raw=true)
<br />
**3. Instalação do Yarn de forma global**
<br />
Abra o prompt de comando como administrador e execute o seguinte comando para que o Yarn será instalado de forma global na máquina:
> npm install --global yarn

**4. Inicialização e configuração da aplicação**
<br />
Abra o prompt de comando no diretório em que deseja gravar sua aplicação e execute o seguinte comando npx instalando todos os pacotes mandatórios:
> npx react-native init NomeDaAplicacao --template react-native-template-typescript

O comando acima executará a inicialização automática de uma aplicação React Native, utilizando um *template* que já tem o Yarn configurado. Assim que finalizado o processo de inicialização, acesse o diretório da aplicação através do comando:
> cd NomeDaAplicacao

Em seguida, utilize o atalho do VisualStudio Code para abrir o fonte da aplicação:
> code .

No VS Code será possível explorar toda a arquitetura de códigos da aplicação, o arquivo principal gerado pelo template é o "App.tsx" (a extensão "tsx" indica um arquivo typescript).
<br />
![enter image description here](https://github.com/hiagoindalecio/TemplateApp/blob/main/OpenVSCode.png?raw=true)
<br />
No VS Code, através do atalho *ctrl + "* é possível a abertura do prompt de comando, então, no prompt de comando execute o comando de atualização de pacotes por precaução:
> yarn

Certifique-se de que o pacote Expo está instalado e atualizado:
> yarn add expo

Inicie o servidor de desenvolvimento através do pacote do Expo:
> yarn expo start

Obs: A inicialização pode ser facilitada ajustando o *script* "start" (package.json) desta maneira:

    {  
	  "scripts": {  
		"start": "expo start"  
	  } 
    }

Então através deste comando, o servidor de desenvolvimento será inicializado:
> yarn start

No prompt de comando será gerado um *IP* de conexão e um *QR code* que pode ser utilizado para a conexão rápida.
[Documentação recomendada](https://reactnative.dev/docs/environment-setup?package-manager=yarn)

**5. Instalação do Expo Go**
<br />
O aplicativo móvel está disponível através do [site oficial](https://expo.dev/client) ou então através das lojas de aplicativos de cada sistema operacional, como [Google Play](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=pt_BR&gl=US) para o Android por exemplo.
Uma vez instalado, certifique-se de que o dispositívo móvel está conectado na mesma rede que o dispositivo rodando o servidor de desenvolvimento e utilize o aplicativo para escanear o *QR code* gerado no passo anterior, uma vez escaneado, a aplicação será montada no dispositivo móvel e a partir deste momento qualquer alteração feita na aplicação através do VS Code refletirá instantaneamente.
<br />
<img src="https://static.expo.dev/static/images/client/expo-go-android.avif" alt="Expo Go" style="height:350px;"/>
<br />

**Tópicos recomendados**
* Hooks
* Context API
* Componentes

[Introdução ao React - site oficial](https://reactnative.dev/docs/intro-react)
