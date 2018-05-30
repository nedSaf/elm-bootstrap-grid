# Bootstrap rendered cards grid
A rendered cards grid with rows in Elm
Renders rows to a given number of columns. Gives the ability to wrap a list
of Html msg with columns and rows.
This will give classes for mobile and tablet, mobile will always have one
element per row and tablet will have half (or close to it with odd numbers) the
number of elements given for desktop.

## Main function explanation
```elm
renderBootstrapCardsGrid : Int -> List (Html msg) -> Html msg
```
The `Int`: Is the number of desired columns in each row.
The `List (Html msg)`: The list of cards that you want to add to the grid.


## Example usage
```elm
renderBootstrapCardsGrid 3 [div [class "card"][], div [class "card"][], div [class "card"][], div [class "card"][], div [class "card"][], div [class "card"][]]
```

This function will return the following:
```html
<div class="container">
  <div class="row">
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
  </div>
  <div class="row">
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
    <div class="col-md-4 col-sm-6 col-xs-12"><div class="card"></div></div>
  </div>
</div>
```
