

- UIKit
- UIScreen
-  applicationFrame Deprecated

Instance Property

# applicationFrame

The frame rectangle for the app window, measured in points.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var applicationFrame: CGRect { get }
```

## Discussion

This property contains the bounds rectangle used by the app window, which may be different than the screen bounds themselves. This rectangle is specified in the current coordinate space, which takes into account any interface rotations in effect for the device. Therefore, the value of this property may change when the device rotates between portrait and landscape orientations.

## See Also

### Deprecated properties

class var main: UIScreen

Returns the screen object representing the device’s screen.

Deprecated

class var screens: [UIScreen]

Returns an array containing all of the screens attached to the device.

Deprecated

var focusedItem: (any UIFocusItem)?

The item that is currently focused.

Deprecated

var focusedView: UIView?

The view that is currently focused.

Deprecated

var supportsFocus: Bool

A Boolean value that indicates whether the screen supports focus-based inputs.

Deprecated

