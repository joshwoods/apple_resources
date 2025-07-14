

- UIKit
- UIUserNotificationAction
-  activationMode Deprecated

Instance Property

# activationMode

The mode in which to run the app when the action is performed.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var activationMode: UIUserNotificationActivationMode { get }
```

## Discussion

If the value in this property is UIUserNotificationActivationMode.foreground, the value of the isAuthenticationRequired property is assumed to be true regardless of its actual value.

## See Also

### Getting the action’s configuration

var isAuthenticationRequired: Bool

A Boolean value indicating whether the user must unlock the device before the action is performed.

Deprecated

var isDestructive: Bool

A Boolean value indicating whether the action is destructive.

Deprecated

var behavior: UIUserNotificationActionBehavior

The custom behavior (if any) that the action supports.

Deprecated

var parameters: [AnyHashable : Any]

A dictionary of additional parameters to include with the action.

Deprecated

