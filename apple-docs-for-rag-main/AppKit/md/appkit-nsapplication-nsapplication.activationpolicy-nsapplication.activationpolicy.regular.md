

- AppKit
- NSApplication
- NSApplication.ActivationPolicy
-  NSApplication.ActivationPolicy.regular 

Case

# NSApplication.ActivationPolicy.regular

The application is an ordinary app that appears in the Dock and may have a user interface.

macOS

``` source
case regular
```

## Discussion

This policy is the default for bundled apps, unless overridden in the `Info.plist`.

## See Also

### Activation Policies

case accessory

The application doesn’t appear in the Dock and doesn’t have a menu bar, but it may be activated programmatically or by clicking on one of its windows.

case prohibited

The application doesn’t appear in the Dock and may not create windows or be activated.

