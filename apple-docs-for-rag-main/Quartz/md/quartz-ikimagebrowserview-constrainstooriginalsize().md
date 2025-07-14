

- Quartz
- IKImageBrowserView
-  constrainsToOriginalSize() 

Instance Method

# constrainsToOriginalSize()

Returns whether the receiver constrains the cell’s image to its original size.

macOS 10.4+

``` source
@MainActor
func constrainsToOriginalSize() -> Bool
```

## Return Value

false if the image is not constrained; otherwise true.

## See Also

### Setting the Appearance

func setCellsStyleMask(Int)

Defines the appearance style of the cells.

func cellsStyleMask() -> Int

Returns the appearance style mask for the cell.

func setConstrainsToOriginalSize(Bool)

Sets whether the receiver constrains the cell’s image to its original size.

func setIntercellSpacing(NSSize)

Sets the spacing between cells in the view.

func intercellSpacing() -> NSSize

Returns the spacing between cells in the view.

