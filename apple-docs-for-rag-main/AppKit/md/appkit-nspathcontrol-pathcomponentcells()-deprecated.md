

- AppKit
- NSPathControl
-  pathComponentCells() Deprecated

Instance Method

# pathComponentCells()

Returns an array of the `NSPathComponentCell` objects currently being displayed.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func pathComponentCells() -> [NSPathComponentCell]
```

Deprecated

Use the pathItems property instead

## Return Value

The array of `NSPathComponentCell` objects.

## See Also

### Managing Path Components

func clickedPathComponentCell() -> NSPathComponentCell?

Returns the clicked cell.

Deprecated

func setPathComponentCells([NSPathComponentCell])

Sets the array of `NSPathComponentCell` objects currently being displayed.

Deprecated

