# React Notes

At it's core React is about building and reusing components to build up an application using Declaritive techniques (defining what state you want rather than how)

# setup react app

recommended to use [create-react-app](https://github.com/facebook/create-react-app), [homepage](https://create-react-app.dev/)

1. Download and install [node.js](https://nodejs.org/en/) (used for create-react-app not to run React)
2. create the react directory with: `npx create-react-app my-app`
3. to run:

```
cd my-app
npm start
```

## JSX

JSX = embedded HTML in javascript code:

```
function App() {
  return (
    <div>
      <h2>Let's get started!</h2>
    </div>
  );
}
```
