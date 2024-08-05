# Angular17Bootstrap5

create a new project, and go into it
```shell
ng new angular17-bootstrap5 --style=scss --ssr=false
cd angular17-bootstrap5
npm install bootstrap --save
npm install jquery --save
npm install popper.js --save
```

install Bootstrap 5 NPM package
```shell
ng new angular17-bootstrap5 --style=scss --ssr=false
cd angular17-bootstrap5
npm install bootstrap@latest-5 --save
npm install jquery --save
npm install popper.js --save
```

check npm installes packages
```shell
npm list

working@ \working\angular17-bootstrap5
+-- bootstrap@5.3.3
+-- jquery@3.7.1
`-- popper.js@1.16.1
```

Import Bootstrap CSS and JS. Edit **angular.json**:

```js
...
"architect": {
  "build": {
    "options": {
      ...
      "styles": [
        "node_modules/bootstrap/dist/css/bootstrap.min.css",
        "src/styles.scss"
      ],
      "scripts": [
          "node_modules/jquery/dist/jquery.min.js",
          "node_modules/bootstrap/dist/js/bootstrap.min.js"
      ]
...
```

