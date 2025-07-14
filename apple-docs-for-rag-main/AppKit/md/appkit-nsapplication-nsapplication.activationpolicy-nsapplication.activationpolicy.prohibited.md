

- AppKit
- NSApplication
- NSApplication.ActivationPolicy
-  NSApplication.ActivationPolicy.prohibited 

Case

# NSApplication.ActivationPolicy.prohibited

The application doesn’t appear in the Dock and may not create windows or be activated.

macOS

``` source
case prohibited
```

## Discussion

This corresponds to the value of the `LSBackgroundOnly` key in the application’s `Info.plist` file being `1`. This is also the default for unbundled executables that don’t have `Info.plist` files.

## See Also

### Activation Policies

case regular

The application is an ordinary app that appears in the Dock and may have a user interface.

case accessory

The application doesn’t appear in the Dock and doesn’t have a menu bar, but it may be activated programmatically or by clicking on one of its windows.

