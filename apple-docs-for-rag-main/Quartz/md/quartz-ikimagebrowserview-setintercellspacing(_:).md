

- Quartz
- IKImageBrowserView
-  setIntercellSpacing(\_:) 

Instance Method

# setIntercellSpacing(\_:)

Sets the spacing between cells in the view.

macOS 10.4+

``` source
@MainActor
func setIntercellSpacing(_ aSize: NSSize)
```

## Parameters 

`aSize`  

The vertical and horizontal spacing between cells.

## Discussion

By default, both values are `10.0` in the receiver’s coordinate system.

## See Also

### Setting the Appearance

func setCellsStyleMask(Int)

Defines the appearance style of the cells.

func cellsStyleMask() -> Int

Returns the appearance style mask for the cell.

func setConstrainsToOriginalSize(Bool)

Sets whether the receiver constrains the cell’s image to its original size.

func constrainsToOriginalSize() -> Bool

Returns whether the receiver constrains the cell’s image to its original size.

func intercellSpacing() -> NSSize

Returns the spacing between cells in the view.

