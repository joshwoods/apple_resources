

- AppKit
- NSPathCellDelegate
-  pathCell(\_:willDisplay:) 

Instance Method

# pathCell(\_:willDisplay:)

Implement this method to customize the Open panel shown by a pop-up–style path.

macOS 10.5+

``` source
@MainActor
optional func pathCell(
    _ pathCell: NSPathCell,
    willDisplay openPanel: NSOpenPanel
)
```

## Parameters 

`pathCell`  

The path cell that sent the message.

`openPanel`  

The Open panel to be displayed.

## Discussion

This method is called before the Open panel is shown but after its allowed file types are set to the cell’s allowed types. At this time, you can further customize the Open panel as required. This method is called only when the style is set to `NSPathStylePopUp`.

Implementation of this method is optional.

