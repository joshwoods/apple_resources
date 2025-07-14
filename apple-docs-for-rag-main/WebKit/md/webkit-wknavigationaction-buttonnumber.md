

- WebKit
- WKNavigationAction
-  buttonNumber 

Instance Property

# buttonNumber

The number of the mouse button that caused the navigation request.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.10+visionOS 2.4+

**macOS**

``` source
@MainActor
var buttonNumber: Int { get }
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
var buttonNumber: UIEvent.ButtonMask { get }
```

## See Also

### Inspecting user actions

var modifierFlags: UIKeyModifierFlags

The modifier keys that were pressed at the time of the navigation request.

