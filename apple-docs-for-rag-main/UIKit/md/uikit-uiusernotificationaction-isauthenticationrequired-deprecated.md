

- UIKit
- UIUserNotificationAction
-  isAuthenticationRequired Deprecated

Instance Property

# isAuthenticationRequired

A Boolean value indicating whether the user must unlock the device before the action is performed.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var isAuthenticationRequired: Bool { get }
```

## Discussion

The value of this property is ignored and treated as a value of true when the value of the activationMode property is set to UIUserNotificationActivationMode.foreground.

If your app uses data protection to encrypt data on disk, consider the data needs of the corresponding action before setting this property to false. For many data protection classes, data remains encrypted and unavailable while the device is locked. If your app needs to access encrypted data to perform a task, you likely need to set this property to true to ensure that the data is accessible.

## See Also

### Getting the action’s configuration

var activationMode: UIUserNotificationActivationMode

The mode in which to run the app when the action is performed.

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

