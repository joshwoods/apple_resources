

- UIKit
- Windows and screens
- UIScreen
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

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

var focusedView: UIView?

The view that is currently focused.

Deprecated

var supportsFocus: Bool

A Boolean value that indicates whether the screen supports focus-based inputs.

Deprecated

### Deprecated notifications

class let didConnectNotification: NSNotification.Name

A notification the system posts when a new screen connects to the device.

Deprecated

class let didDisconnectNotification: NSNotification.Name

A notification the system posts when a screen disconnects from the device.

Deprecated

