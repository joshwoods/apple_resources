

- Quartz
- IKImageBrowserView
-  setCellsStyleMask(\_:) 

Instance Method

# setCellsStyleMask(\_:)

Defines the appearance style of the cells.

macOS 10.4+

``` source
@MainActor
func setCellsStyleMask(_ mask: Int)
```

## Parameters 

`mask`  

An integer bit mask. A mask can be specified by combining any of the options described in Cell Appearance Style Masks using the C bitwise `OR` operator.

## See Also

### Setting the Appearance

func cellsStyleMask() -> Int

Returns the appearance style mask for the cell.

func setConstrainsToOriginalSize(Bool)

Sets whether the receiver constrains the cell’s image to its original size.

func constrainsToOriginalSize() -> Bool

Returns whether the receiver constrains the cell’s image to its original size.

func setIntercellSpacing(NSSize)

Sets the spacing between cells in the view.

func intercellSpacing() -> NSSize

Returns the spacing between cells in the view.

