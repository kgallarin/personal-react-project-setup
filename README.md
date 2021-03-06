# Linting and Prettify Setup

Default project setup including modules, linters and README

# Using react-redux

Redux modules for yarn installation :

```
$yarn add react-redux redux-thunk redux redux-logger redux-promise-middleware
```

if you are using chrome extension for redux-store :

```
let composeEnhancers = compose;
let middlewares = [reduxThunk]

if(process.env.NODE_ENV !== 'production'){
  const logger = reduxLogger

  middlewares = [...middlewares,logger]

  composeEnhancers = window.__REDUX_DEVTOOLS_EXTENSION_COMPOSE__ || compose
}

export default () => {
  return createStore(
    reducers,
    {},
    composeEnhancers(applyMiddleware(...middlewares))
  )
}

```

# Husky for prettify version control

Setup after installing inside package.json

```
$node node_modules/husky/bin/install.js
```

# Installing json-server with your app

Inside your package.json :

```
"start": "npm-run-all -p watch-css start-js & npm run apiserver"
```

also add this for rehydrating npm apiserver script

```
apiserver": "json-server --watch --port 3001 api/your_json_name.json`
```

# Installing Bootstrap

```
$npm install react-bootstrap --save
$npm install bootstrap --save
```

and make sure you also import stylesheets :

```
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap/dist/css/bootstrap-theme.css';
```
# Husky

Upgrade husky

```
$npm i husky@0.15.0-rc.3 --save-dev

or

$yarn add husky@next --dev
```

make sure "pre-commit" is existing before running :

```
$node_modules/.bin/husky-upgrade
```
