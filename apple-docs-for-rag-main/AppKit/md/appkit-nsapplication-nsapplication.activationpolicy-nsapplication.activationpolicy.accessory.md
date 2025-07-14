

- AppKit
- NSApplication
- NSApplication.ActivationPolicy
-  NSApplication.ActivationPolicy.accessory 

Case

# NSApplication.ActivationPolicy.accessory

The application doesn’t appear in the Dock and doesn’t have a menu bar, but it may be activated programmatically or by clicking on one of its windows.

macOS

``` source
case accessory
```

## Discussion

This corresponds to value of the `LSUIElement` key in the application’s `Info.plist` being `1`.

## See Also

### Activation Policies

case regular

The application is an ordinary app that appears in the Dock and may have a user interface.

case prohibited

The application doesn’t appear in the Dock and may not create windows or be activated.

