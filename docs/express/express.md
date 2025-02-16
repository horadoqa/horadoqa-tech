# EXPRESS

Agora, você pode instalar pacotes ou dependências que seu projeto necessite. Por exemplo, para instalar o Express, um framework popular para Node.js, use:

```bash
npm install express
```

Criar o arquivo principal (geralmente index.js)


Crie o arquivo que será o ponto de entrada do seu projeto. Por exemplo, crie um arquivo chamado index.js:

```bash
touch index.js
```

Dentro desse arquivo, você pode começar a escrever o código do seu servidor ou aplicação.

Exemplo básico de um servidor com Express:

```javascript
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Olá, Mundo!');
});

app.listen(port, () => {
  console.log(`Servidor rodando na porta ${port}`);
});
```

6. Rodar o projeto

Para rodar o projeto, basta executar o seguinte comando no terminal:

```bash
node index.js
```

Isso iniciará o servidor e você verá a mensagem no console indicando que o servidor está rodando.

Agora, se você acessar http://localhost:3000 no navegador, verá a mensagem "Olá, Mundo!".


## Desenvolvimento contínuo

À medida que o projeto cresce, você pode adicionar mais dependências, módulos e funcionalidades. Se for necessário monitorar mudanças em tempo real, é comum usar uma ferramenta como o nodemon para reiniciar automaticamente o servidor quando alterações forem feitas.

Para instalar o nodemon:

```bash
npm install --save-dev nodemon
```

Agora, você pode rodar o servidor com o nodemon:

```bash
npx nodemon index.js
```

Isso fará com que seu servidor seja reiniciado automaticamente sempre que você modificar o código.