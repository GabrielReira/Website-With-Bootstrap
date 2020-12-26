# Website-With-Bootstrap

## :desktop_computer: Sobre o projeto

Este projeto foi criado enquanto eu aprendia o básico sobre Bootstrap e suas diversas funcionalidades.
Esse website foi completamente realizado utilizando  os arquivos fonte do [Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/download/) com Sass.

Durante todo o processo, não copiei uma linha sequer dos códigos na documentação do Bootstrap, foram todos feitos aos poucos
e estudando cada detalhe.

Apesar de ser um website bastante simplório (apenas com finalidade de aprendizado), ele foi pensado nos deficientes visuais,
portanto, todo o website foi realizado baseado nas tecnologias assistivas, como os leitores de tela.


---


## :rocket: Tecnologias utilizadas
* HTML 5
* Sass (3.7.4)
* Bootstrap (4.5.2)
* jQuery (3.5.1)
* Popper.js (1.16.1)


---


## :gear: Pré-requisitos e ferramentas

### Pré-requisitos :detective:
- Possuir o [Git](https://git-scm.com/downloads) instalado e configurado no computador;
- Possuir um gerenciador de pacotes, seja o [Yarn](https://yarnpkg.com/) ou [npm](https://www.npmjs.com/);
- Por fim, possuir o [Node.js](https://nodejs.org/en/) instalado no computador.

### Clonando o repositório :cyclone:
No terminal git:
```sh
    # Clonar o repositório
    $ git clone https://github.com/GabrielReira/Website-With-Bootstrap.git
    # Entrar no diretório
    $ cd website-with-bootstrap
```

### Instalando pacotes :package:
Primeiramente, você precisa baixar e instalar as principais ferramentas no seu computador.
```sh
    # Para baixar o Bootstrap
    $ npm install bootstrap
    # Para instalar o jQuery
    $ npm install jquery
    # Para instalar Popper.js
    $ npm install popper.js
```
O Bootstrap exigirá um compilador de Sass, então também é necessário fazer sua instalação.
```sh
    # Instalando o Sass
    $ npm install -g sass
```
Para mais detalhes de instalação do Bootstrap na sua máquina você pode acessar o próprio site do
[Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/download/), ou [esse do npm](https://www.npmjs.com/package/bootstrap)
que aborda maneiras rápidas de instalação do pacote Bootstrap através do próprio npm, yarn, Composer, NuGet etc.


---


## :fire: Inicialização do projeto

Primeiro, acesse o diretório onde o repositório foi clonado, então instale os módulos listados como dependências
no arquivo [package.json](https://github.com/GabrielReira/Website-With-Bootstrap/blob/master/package.json).
```sh
    # Acesse o diretório
    $ cd C:\Users\gabriel\Desktop\Website-With-Bootstrap
    # Instale as dependências
    $ npm install
```

**Tenha em mente que para fazer qualquer alteração trabalhando com Bootstrap é necessário compilar os**
**arquivos modificados para que o seu navegador possa interpretá-los da maneira correta.**

### Compilando arquivos scss :brain:
Crie uma pasta de nome 'compiler' dentro de 'node_modules/bootstrap', que é onde ficará os arquivos compilados de scss
para css. Então compile o arquivo scss num arquivo css para o navegador poder interpretá-lo.
```sh
    # Compilando o arquivo scss em css
    $ sass --watch node_modules/bootstrap/scss:node_modules/bootstrap/compiler
```

### Compilando pasta styles :art:
Para fazer qualquer alteração no arquivo
[style.css](https://github.com/GabrielReira/Website-With-Bootstrap/blob/master/web/styles/style.css) é necessário
compilar a pasta styles no sass.
```sh
    # Compilando a pasta styles
    $ sass --watch web/styles:node_modules/bootstrap/compiler
```

### Compilando Font Awesome :abcd:
O pacote do Font Awesome já vem com um diretório onde fica os arquivos scss e outro com os arquivos já compilados em css,
então não precisa compilá-los para o diretório 'node_modules/bootstrap/compiler'.
```sh
    # Compilando o Font Awesome
    $ sass --watch node_modules/@fortawesome/fontawesome-free/scss:node_modules/@fortawesome/fontawesome-free/css
```

### Compilando tudo com apenas um comando :man_technologist:
Caso você realize muitas alterações no projeto, é possível compilar todos os arquivos de uma só vez.
```sh
    # Compilando todos os arquivos
    $ sass --watch node_modules/bootstrap/scss:node_modules/bootstrap/compiler web/styles:node_modules/bootstrap/compiler node_modules/@fortawesome/fontawesome-free/scss:node_modules/@fortawesome/fontawesome-free/css
```

**Obs.: Fique atento caso você troque as pastas de diretório ou renomeie algum arquivo.**


---


## :scroll: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/GabrielReira/Website-With-Bootstrap/blob/master/LICENSE) para mais detalhes.

---

<p align="center"><strong>Por <a href="https://www.linkedin.com/in/gabriel-reira/">Gabriel Reira</a></strong></p>
