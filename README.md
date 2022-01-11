# Interactive Readmes with Devbook

This is an example of how Devbook can be used to build interactive readmes.

**This readme has attached a full-fledged VM to it that both the author and a reader can use.**

Readmes built with Devbooks are great because they allow developers to play with the third-party libraries and packages without any setup. They can do it right inside the Devbook.

## It's interactive!

Every piece of code here can edited and executed. You can deploy any conainer to the attached VM  and run them alongside. In this readme, we are using a prebuilt Next.js template. You can see the environment running in the left sidebar.

## It's all markdown!

Really. Devbook can serialize and commit this readme to a simple markdown `README` file in your repo. Look at <https://github.com/DevbookHQ/interactive-readme>. The commited readme is this Devbook. Of course, Devbook can pull the readme from your repo as well.

## It has multiplayer!

Devbook support collaborative editing. Open this URL in another window and you'll see each other's cursor.

Each session has it's own VM.

## Readme we are about to write

The readme we are about to write is for a React library called [Splitter](https://github.com/DevbookHQ/splitter). Splitter is a React component that allows you to split and resize view. We will use the `nextjs` template to show how Splitter works.

# \
Splitter

Splitter is a React component that allows you to split views into resizable panels. Similar to tabs in Visual Studio Code, for example.

## Installation

```sh {"template-id":"nextjs-v11-components"}
npm i @devbookhq/splitter
```

## Interactive Demo

> Make sure to run the above shell cell first

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-f932e410b823.o.usedevbook.com/">

The demo you've just interacted with, in the above iframe, is running in the VM attached to this Devbook document.

You can customize it however you want: Open the `components/Horizontal.tsx` file and change the "Tile 1" text to "Tile 0". The iframe will update.

## Examples

**Each of the following code snippets is an actual file the `pages` directory that you can edit.**

When you add a Next.js code cell (by pressing '/'), Devbook automatically creates an underlying file in the `pages` directory so you can easily render it via iframe.

Notice that we are basically creating an interactive readme with a built-in Next.js app without creting any Codesandbox/Replit/StackBlitz/etc project. We didn't have to leave Devbook to write or edit the code and run it.

### Horizontal split

```tsx {"cell-id":"mxbsj52b","document-env-id":"1ad1629e","template-id":"nextjs-v11-components","cell-name":"Untitled"}
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

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-f932e410b823.o.usedevbook.com/Untitled">### Vertical split

```tsx {"cell-id":"q298mw5j","document-env-id":"1ad1629e","template-id":"nextjs-v11-components","cell-name":"Untitled-u7c"}
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

<meta cell-type="iframe" src="https://3000-cky7n1gxo23374808ij62d9h33y_1ad1629e-f932e410b823.o.usedevbook.com/Untitled-u7c">