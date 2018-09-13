# Linting and Prettify Setup

Default project setup including modules, linters and README

# Using react-redux

Redux modules for yarn installation :

```
$yarn add react-redux redux-thunk redux redux-logger redux-promise-middleware
```

if you are using chrome extension for redux-store :

```
 export default () => createStore({
    your_root_reducer,
    REDUX STORE EXTENSION window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__(),
    applyMiddleWare([...middlewares])
})
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
$installing bootstrap
$npm install react-bootstrap --save
$npm install bootstrap --save
```

and make sure you also import stylesheets :

```
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap/dist/css/bootstrap-theme.css';
```

# Need Sliders

Visit :

[react-slick](https://github.com/akiran/react-slick)

# Husky

Upgrade husky

```
$npm i husky@0.15.0-rc.3 --save-dev
$yarn add husky@next --dev
```

make sure "pre-commit" is existing before running :

```
$node_modules/.bin/husky-upgrade
```

[react-slick](https://github.com/akiran/react-slick)

# Author

- **Kevin M. Gallarin** - _Frontend Developer_ - [Linkedin](https://www.linkedin.com/in/kmgallarin/)
