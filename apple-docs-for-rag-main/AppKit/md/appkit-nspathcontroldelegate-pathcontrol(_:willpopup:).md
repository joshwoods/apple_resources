

- AppKit
- NSPathControlDelegate
-  pathControl(\_:willPopUp:) 

Instance Method

# pathControl(\_:willPopUp:)

Implement this method to customize the menu of a pop-up–style path.

macOS 10.5+

``` source
@MainActor
optional func pathControl(
    _ pathControl: NSPathControl,
    willPopUp menu: NSMenu
)
```

## Parameters 

`pathControl`  

The path control displaying the pop-up menu.

`menu`  

The pop-up menu to be displayed.

## Discussion

This method is called before the pop-up menu is shown. At this time, you can further customize the menu as required, adding and removing items. This method is called only when the style is set to `NSPathStylePopUp`. Implementation of this method is optional.

## See Also

### Customizing a Pop-Up–Style Path

func pathControl(NSPathControl, willDisplay: NSOpenPanel)

Implement this method to customize the Open panel shown by a pop-up–style path.

