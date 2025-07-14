

- UIKit
- UIScreen
-  screens Deprecated

Type Property

# screens

Returns an array containing all of the screens attached to the device.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedtvOSDeprecated

``` source
@MainActor
class var screens: [UIScreen] { get }
```

Deprecated

Use openSessions on the shared app object to find scenes for other screens.

## Return Value

An array of `UIScreen` objects.

## Discussion

The returned array includes the main screen plus any additional screens connected to the device. The main screen is always at index `0`.

Not all devices support external displays. iPhone and iPod touch devices with Retina displays and iPads support external displays. Older devices, such as the iPhone 3GS, don’t support external displays.

## See Also

### Deprecated properties

class var main: UIScreen

Returns the screen object representing the device’s screen.

Deprecated

var applicationFrame: CGRect

The frame rectangle for the app window, measured in points.

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

