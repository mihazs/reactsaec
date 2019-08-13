### Configuração Linux

#### Visual Studio

Primeiramente, faça update dos índices de pacotes e instale as dependências:

```bash
sudo apt update
sudo apt install software-properties-common apt-transport-https wget
```

Em seguida importe as chaves GPG usando o seguinte wget:

```bash
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
```

Depois habilite o repositório VSCode:

```bash
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```

##### Extensões do VSCode

Os complementos nesta IDE são mais que recursos extras, elas conseguem ajudar o desenvolvedor a criar seus códigos em praticamente qualquer linguagem e isso, por si só, já é algo importante.

Para ativar e instalar uma nova extensão, basta clicar no último ícone da barra lateral de ferramentas do Visual Studio Code. Será mostrado inicialmente as extensões mais populares. Para instalar, é só escolher a extensão, verificar sua documentação básica e clicar no botão “Install” ou "Instalar". Depois disso é só começar a utilizar o novo recurso.

Extensões recomendadas:
1. ESLint
2. ES7 React/Redux/React-Native/JS snippets
3. prisma.vscode-graphql

#### Instalação do NodeJS

Abre o terminal e digite:

```bash
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```

##### Instalando o yarn

Após instalar o node abra o terminal e digite:

```bash
npm install -g yarn
```

##### Instalando create-react-app

Abra o terminal e digite:

```bash
yarn global add create-react-app
```

ou, se não funcionar:

```bash
npm install -g create-react-app
```

Qualquer dúvida: mihael.zaminsousa@gmail.com
