

- UIKit
- UIScreen
-  focusedView Deprecated

Instance Property

# focusedView

The view that is currently focused.

iOS 9.0–15.0DeprecatediPadOS 9.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 9.0–15.0Deprecated

``` source
@MainActor
weak var focusedView: UIView? { get }
```

## Discussion

When a view has focus, this property contains that view. When the focus is on an item that is not a view, the view in this property is the one that contains the item. This property is `nil` when nothing is currently focused on the screen.

## See Also

### Deprecated properties

class var main: UIScreen

Returns the screen object representing the device’s screen.

Deprecated

class var screens: [UIScreen]

Returns an array containing all of the screens attached to the device.

Deprecated

var applicationFrame: CGRect

The frame rectangle for the app window, measured in points.

Deprecated

var focusedItem: (any UIFocusItem)?

The item that is currently focused.

Deprecated

var supportsFocus: Bool

A Boolean value that indicates whether the screen supports focus-based inputs.

Deprecated

