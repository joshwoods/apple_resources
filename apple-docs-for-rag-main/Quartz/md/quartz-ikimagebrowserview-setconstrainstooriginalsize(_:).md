

- Quartz
- IKImageBrowserView
-  setConstrainsToOriginalSize(\_:) 

Instance Method

# setConstrainsToOriginalSize(\_:)

Sets whether the receiver constrains the cell’s image to its original size.

macOS 10.4+

``` source
@MainActor
func setConstrainsToOriginalSize(_ flag: Bool)
```

## Parameters 

`flag`  

A flag that specifies whether to constrain the image. The default value is false.

## See Also

### Setting the Appearance

func setCellsStyleMask(Int)

Defines the appearance style of the cells.

func cellsStyleMask() -> Int

Returns the appearance style mask for the cell.

func constrainsToOriginalSize() -> Bool

Returns whether the receiver constrains the cell’s image to its original size.

func setIntercellSpacing(NSSize)

Sets the spacing between cells in the view.

func intercellSpacing() -> NSSize

Returns the spacing between cells in the view.

