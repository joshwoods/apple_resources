

- AppKit
- NSPathControlDelegate
-  pathControl(\_:willDisplay:) 

Instance Method

# pathControl(\_:willDisplay:)

Implement this method to customize the Open panel shown by a pop-up–style path.

macOS 10.5+

``` source
@MainActor
optional func pathControl(
    _ pathControl: NSPathControl,
    willDisplay openPanel: NSOpenPanel
)
```

## Parameters 

`pathControl`  

The path control displaying the Open panel.

`openPanel`  

The Open panel to be displayed.

## Discussion

This method is called before the Open panel is shown but after its allowed file types are set to the cell’s allowed types. At this time, you can further customize the Open panel as required. This method is called only when the style is set to `NSPathStylePopUp`. Implementation of this method is optional.

## See Also

### Customizing a Pop-Up–Style Path

func pathControl(NSPathControl, willPopUp: NSMenu)

Implement this method to customize the menu of a pop-up–style path.

