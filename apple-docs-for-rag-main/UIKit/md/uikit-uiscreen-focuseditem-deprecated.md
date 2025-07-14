

- UIKit
- UIScreen
-  focusedItem Deprecated

Instance Property

# focusedItem

The item that is currently focused.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 10.0–15.0Deprecated

``` source
@MainActor
weak var focusedItem: (any UIFocusItem)? { get }
```

## Discussion

If this item is not a view, the focusedView property is set to the view that contains the item.

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

var focusedView: UIView?

The view that is currently focused.

Deprecated

var supportsFocus: Bool

A Boolean value that indicates whether the screen supports focus-based inputs.

Deprecated

