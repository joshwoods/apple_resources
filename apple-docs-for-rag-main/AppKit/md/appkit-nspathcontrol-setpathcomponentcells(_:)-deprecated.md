

- AppKit
- NSPathControl
-  setPathComponentCells(\_:) Deprecated

Instance Method

# setPathComponentCells(\_:)

Sets the array of `NSPathComponentCell` objects currently being displayed.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func setPathComponentCells(_ cells: [NSPathComponentCell])
```

Deprecated

Use the pathItems property instead

## Parameters 

`cells`  

An array of `NSPathComponentCell` objects.

## Discussion

Each item in the array must be an instance of `NSPathComponentCell` or a subclass thereof. You cannot set this value to `nil`, but you can set it to an empty array using, for example, `[NSArray array]`.

## See Also

### Managing Path Components

func clickedPathComponentCell() -> NSPathComponentCell?

Returns the clicked cell.

Deprecated

func pathComponentCells() -> [NSPathComponentCell]

Returns an array of the `NSPathComponentCell` objects currently being displayed.

Deprecated

