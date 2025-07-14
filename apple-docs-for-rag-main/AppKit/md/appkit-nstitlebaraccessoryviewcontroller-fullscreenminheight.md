

- AppKit
- NSTitlebarAccessoryViewController
-  fullScreenMinHeight 

Instance Property

# fullScreenMinHeight

The visual minimum height of an accessory view that displays below the title bar when the window is in full screen mode.

macOS 10.10+

``` source
@MainActor
var fullScreenMinHeight: CGFloat { get set }
```

## Discussion

The fullScreenMinHeight property applies only to an `NSTitlebarAccessoryViewController` object in which layoutAttribute is set to NSLayoutConstraint.Attribute.bottom. The minimum height you set determines how much of your accessory view is visible when the menu bar is hidden during full screen mode. By default, the minimum height is `0`, which means that the accessory view is hidden when the menu bar is hidden. When a user reveals the menu bar in this scenario, the accessory view is also revealed.

To persistently show a portion of the accessory view, set this property to a value greater than `0`. For example, if you have a fixed height accessory view, you can set fullScreenMinHeight to `view.frame.size.height` to show the view regardless of whether the menu bar is hidden. Note that the view’s height is never actually changed when it is hidden or revealed; instead, it is automatically clipped by an internal clip view.

## See Also

### Configuring a Title Bar Accessory View Controller

var layoutAttribute: NSLayoutConstraint.Attribute

The location of the accessory view, in relation to the window’s title bar.

