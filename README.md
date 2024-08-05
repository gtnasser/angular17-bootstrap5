# Angular17Bootstrap5

create a new project, and go into it
```shell
ng new angular17-bootstrap5 --style=scss --ssr=false
cd angular17-bootstrap5
```

install Bootstrap 5 NPM package running ```npm install bootstrap@latest-5 --save```

Edit **angular.json** to import Bootstrap CSS and JS.

```js
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

Now let´s copy the code below from Bootstrap Docs and paste into **app.component.html**:
```html
<div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false">
    Dropdown button
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
    <li><a class="dropdown-item" href="#">Action</a></li>
    <li><a class="dropdown-item" href="#">Another action</a></li>
    <li><a class="dropdown-item" href="#">Something else here</a></li>
  </ul>
</div>

<br>

<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
  Launch static backdrop modal
</button>

<!-- Modal -->
<div class="modal fade" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="staticBackdropLabel">Modal title</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        Modal body content here
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Understood</button>
      </div>
    </div>
  </div>
</div>
```

That´s it, fully Bootstrap 5 running into a Angular 17 project.

If it don´t run on ```ng serve```, try execute ```ng build``` before running ```ng serve``` again.

