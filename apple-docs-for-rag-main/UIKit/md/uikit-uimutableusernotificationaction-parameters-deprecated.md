

- UIKit
- UIMutableUserNotificationAction
-  parameters Deprecated

Instance Property

# parameters

A dictionary of additional parameters to include with the action.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var parameters: [AnyHashable : Any] { get set }
```

## Discussion

Use this dictionary to specify any behavior-specific data for the action. For example, the `UIUserNotificationActionBehaviorTextInput` behavior supports the `UIUserNotificationTextInputActionButtonTitleKey` key, which lets you customize the title of the button displayed by the text input interface.

## See Also

### Configuring the action’s behavior

var activationMode: UIUserNotificationActivationMode

The mode in which to run the app when the action is performed.

Deprecated

var isAuthenticationRequired: Bool

A Boolean value indicating whether the user must unlock the device before the action is performed.

Deprecated

var isDestructive: Bool

A Boolean value indicating whether the action is destructive.

Deprecated

var behavior: UIUserNotificationActionBehavior

The custom behavior (if any) that the action supports.

Deprecated

