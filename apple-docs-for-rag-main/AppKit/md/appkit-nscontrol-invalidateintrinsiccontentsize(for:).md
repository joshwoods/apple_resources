

- AppKit
- NSControl
-  invalidateIntrinsicContentSize(for:) 

Instance Method

# invalidateIntrinsicContentSize(for:)

Notifies the control that the intrinsic content size for its cell is no longer valid.

macOS 10.7+

``` source
@MainActor
func invalidateIntrinsicContentSize(for cell: NSCell)
```

## Parameters 

`cell`  

The cell whose intrinsic content size has changed.

## Discussion

Controls determine their intrinsic content size based on the cell size for a given bounds returned by their cell. When the content of the cell changes in a way that would change the return value of cellSize(forBounds:), the cell needs to call this method to notify its control that its intrinsic size is no longer valid.

