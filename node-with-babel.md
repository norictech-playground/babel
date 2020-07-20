## NodeJS with Babel

- install nodemon
```
yarn add nodemon -g
```

- install babel and the needed presets
```
yarn add @babel/core @babel/preset-env @babel/preset-stage-3
```

- edit `package.json`
```
...
"scripts": {
  "start": "nodemon --exec babel-node your-server.js"
}
...
```

- create a new file called `.babelrc` in the root directory, and add these following of code:
```
{
  "presets": [
    "env",
    "stage-3"
  ]
}
```
