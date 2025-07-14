

- UIKit
- UIUserNotificationAction
-  behavior Deprecated

Instance Property

# behavior

The custom behavior (if any) that the action supports.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var behavior: UIUserNotificationActionBehavior { get }
```

## Discussion

The default value of this property is UIUserNotificationActionBehavior.default.

## See Also

### Getting the action’s configuration

var activationMode: UIUserNotificationActivationMode

The mode in which to run the app when the action is performed.

Deprecated

var isAuthenticationRequired: Bool

A Boolean value indicating whether the user must unlock the device before the action is performed.

Deprecated

var isDestructive: Bool

A Boolean value indicating whether the action is destructive.

Deprecated

var parameters: [AnyHashable : Any]

A dictionary of additional parameters to include with the action.

Deprecated

