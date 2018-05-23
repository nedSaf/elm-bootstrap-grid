# Bootstrap rendered grid
A rendered grid with rows in Elm

## Example usage
```elm
renderBootstrapGrid 3 [div [][], div [][], div [][]]
```

This function will return the following:
```html
<div class="row">
  <div class="col-md-4 col-sm-6 col-xs-12"></div>
  <div class="col-md-4 col-sm-6 col-xs-12"></div>
  <div class="col-md-4 col-sm-6 col-xs-12"></div>
</div>
```
