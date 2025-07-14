

- AppKit
- NSPathControl
-  clickedPathComponentCell() Deprecated

Instance Method

# clickedPathComponentCell()

Returns the clicked cell.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func clickedPathComponentCell() -> NSPathComponentCell?
```

Deprecated

Use the clickedPathItem property instead

## Return Value

The component cell that was clicked.

## Discussion

The value returned is generally valid only when the action or double action is being sent.

Note

In OS X v10.5 and earlier the returned value was \[nil\] if no cell had been clicked. In OS X v10.6, the folder of the cell that the user selected is returned instead.

## See Also

### Managing Path Components

func pathComponentCells() -> [NSPathComponentCell]

Returns an array of the `NSPathComponentCell` objects currently being displayed.

Deprecated

func setPathComponentCells([NSPathComponentCell])

Sets the array of `NSPathComponentCell` objects currently being displayed.

Deprecated

