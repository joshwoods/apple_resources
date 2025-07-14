

- UIKit
- UIUserNotificationAction
-  isDestructive Deprecated

Instance Property

# isDestructive

A Boolean value indicating whether the action is destructive.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var isDestructive: Bool { get }
```

## Discussion

Use this property to signal to the user whether the action causes destructive behavior to the user’s data or the app. When the value of this property is true, the system displays the corresponding button differently to indicate that the action is destructive.

The default value of this property is false.

## See Also

### Getting the action’s configuration

var activationMode: UIUserNotificationActivationMode

The mode in which to run the app when the action is performed.

Deprecated

var isAuthenticationRequired: Bool

A Boolean value indicating whether the user must unlock the device before the action is performed.

Deprecated

var behavior: UIUserNotificationActionBehavior

The custom behavior (if any) that the action supports.

Deprecated

var parameters: [AnyHashable : Any]

A dictionary of additional parameters to include with the action.

Deprecated

