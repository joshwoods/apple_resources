

- UIKit
- UIScreen
-  main 

Type Property

# main

Returns the screen object representing the device’s screen.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+tvOS

``` source
@MainActor
class var main: UIScreen { get }
```

## Return Value

The screen object for the device.

## Discussion

Apple discourages the use of this symbol. Use a UIScreen instance found through context instead. For example, reference the screen that displays a view through the screen property on the window scene managing the window containing the view.

## See Also

### Deprecated properties

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

