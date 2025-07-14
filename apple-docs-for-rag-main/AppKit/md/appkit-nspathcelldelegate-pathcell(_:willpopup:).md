

- AppKit
- NSPathCellDelegate
-  pathCell(\_:willPopUp:) 

Instance Method

# pathCell(\_:willPopUp:)

Implement this method to customize the menu of a pop-up–style path.

macOS 10.5+

``` source
@MainActor
optional func pathCell(
    _ pathCell: NSPathCell,
    willPopUp menu: NSMenu
)
```

## Parameters 

`pathCell`  

The path cell that sent the message.

`menu`  

The pop-up menu to be displayed.

## Discussion

This method is called before the pop-up menu is shown. At this time, you can further customize the menu as required, adding and removing items. This method is called only when the style is set to `NSPathStylePopUp`.

Implementation of this method is optional.

