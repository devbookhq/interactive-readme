# lnteractive Readmes with Devbook

This is an example of how Devbook can be used to build interactive readmes.

**This readme has attached a full-fledged VM to it that both the author and a reader can use.**

Readmes built with Devbooks are great because they allow developers to play with the third-party libraries and packages without any setup. They can do it right inside the Devbook.

## It's interactive!

Every piece of code here can edited and executed. You can deploy any container to the attached VM  and run them alongside. In this readme, we are using a prebuilt Next.js template. You can see the environment running in the left sidebar.

## It's all markdown!

Really. Devbook can serialize and commit this readme to a simple markdown `README` file in your repo. Look at <https://github.com/DevbookHQ/interactive-readme>. The commited readme is this Devbook. Of course, Devbook can pull the readme from your repo as well.

## It has multiplayer!

Devbook supports collaborative editing. Open this URL in another window and you'll see a new cursor.

Each session has it's own VM.

## Readme we are about to write

The readme we are about to write is for a React library called [Splitter](https://github.com/DevbookHQ/splitter). Splitter is a React component that allows you to split and resize view. We will use the `nextjs` template to show how Splitter works.

---

# Splitter

Splitter is a React component that allows you to split views into resizable panels. Similar to tabs in Visual Studio Code, for example.

## Installation

```sh {"template-id":"nextjs-v11-components"}
npm i @devbookhq/splitter
```

## Interactive Demo

> Make sure to run the above shell command first

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-2083b784ec38.o.usedevbook.com/">


The demo you've just interacted with, in the  iframe above, is running in the VM attached to this Devbook document.

You can customize it however you want: Open the `components/Horizontal.tsx` file and change the "Tile 1" text to "Tile 0". The iframe will update.

## Examples

**Each of the following code cells is an actual file the `pages` directory that you can edit. Or edit the code cell directly here.**

When you add a Next.js code cell (by pressing '/'), Devbook automatically creates an underlying file in the `pages` directory so you can easily render it via iframe.

Notice that we are basically creating an interactive readme with a built-in Next.js app without creting any Codesandbox/Replit/StackBlitz/etc project. We didn't have to leave Devbook to write or edit the code and run it.

---

### Horizontal split

```tsx {"cell-id":"09zcxpwy","cell-name":"cc.tsx","document-env-id":"1ad1629e","template-id":"nextjs-v11-components"}
import Splitter, { SplitDirection } from '@devbookhq/splitter'

function MyComponent() {
  return (
    <Splitter>
      <div className="tile">Tile 1</div>
      <div className="tile">Tile 2</div>
    </Splitter>
  );
}

export default MyComponent
```

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-e53ceeb549dc.o.usedevbook.com/cc">

### Vertical split

```tsx {"cell-id":"efmyjeme","cell-name":"cc-a3j.tsx","document-env-id":"1ad1629e","template-id":"nextjs-v11-components"}
import Splitter, { SplitDirection } from '@devbookhq/splitter'

function MyComponent() {
  return (
    <Splitter
      direction={SplitDirection.Vertical}  
    >
      <div className="tile">Tile 1</div>
      <div className="tile">Tile 2</div>
    </Splitter>
  );
}

export default MyComponent
```

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-e53ceeb549dc.o.usedevbook.com/cc-a3j">


 

```sh {"template-id":"nodejs-v16"}
npm i node-fetch
```

```ts {"cell-id":"8q0vf70w","cell-name":"cc.js","document-env-id":"6f521b19","template-id":"nodejs-v16"}
// import fetch from 'node-fetch';

// const response = await fetch('https://github.com/');
// const body = await response.text();

// console.log(body);

// import http from 'http';

// function handler(req, res) {
//   res.writeHead(200);
//   res.end('Hello World!');
// }

// const server = http.createServer(handler);
// setTimeout(() => {
//   // console.log('hello')
// }, 5000)

// setTimeout(() => {
//   console.log('Closing server...');
//   server.close();
//   console.log('Closed');
// }, 1000 * 60);

// console.log('Starting server...');
// server.listen(3000);

console.log('Hello world')
```

```sh {"template-id":"nodejs-v16","run-on-start":"true"}
node src/cc.js
```