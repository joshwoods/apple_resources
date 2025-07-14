

- WebKit
- WKNavigationAction
-  modifierFlags 

Instance Property

# modifierFlags

The modifier keys that were pressed at the time of the navigation request.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.10+visionOS 2.4+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
var modifierFlags: UIKeyModifierFlags { get }
```

**macOS**

``` source
@MainActor
var modifierFlags: NSEvent.ModifierFlags { get }
```

## See Also

### Inspecting user actions

var buttonNumber: UIEvent.ButtonMask

The number of the mouse button that caused the navigation request.

