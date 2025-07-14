

- AppKit
- NSTitlebarAccessoryViewController
-  layoutAttribute 

Instance Property

# layoutAttribute

The location of the accessory view, in relation to the window’s title bar.

macOS 10.10+

``` source
@MainActor
var layoutAttribute: NSLayoutConstraint.Attribute { get set }
```

## Discussion

The default value of this property is NSLayoutConstraint.Attribute.bottom, which means that the accessory view should display below the title bar. You can also set this property to NSLayoutConstraint.Attribute.right or (in apps linked on macOS 10.11 or later) NSLayoutConstraint.Attribute.left. All other values are invalid and will cause an assertion to be raised.

Note

In an app linked on macOS 10.11 or later, setting layoutAttribute to NSLayoutConstraint.Attribute.right does not right indent toolbar items unless the window’s titleVisibility property is equal to NSWindow.TitleVisibility.hidden.

## See Also

### Configuring a Title Bar Accessory View Controller

var fullScreenMinHeight: CGFloat

The visual minimum height of an accessory view that displays below the title bar when the window is in full screen mode.

