

- UIKit
- UILocalNotification
-  category Deprecated

Instance Property

# category

The name of a group of actions to display in the alert.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var category: String? { get set }
```

## Discussion

The value of this property is the category name associated with a registered UIUserNotificationSettings object. When the alert for the local notification is displayed, the system uses the string you specify to look up the group and retrieve its actions. It then adds a button to the alert for each action defined by the group. When the user taps one of those buttons, the app is woken up (or launched) and given a chance to perform the designated action. If the specified category name does not belong to a registered group of actions, the alert does not display any additional action buttons.

Specifying custom actions is optional. The value of this property is `nil` by default.

## See Also

### Composing the alert

var alertBody: String?

The message displayed in the notification alert.

Deprecated

var alertAction: String?

The title of the action button or slider.

Deprecated

var alertTitle: String?

A short description of the reason for the alert.

Deprecated

var hasAction: Bool

A Boolean value that controls whether the notification shows or hides the alert action.

Deprecated

var alertLaunchImage: String?

Identifies the image used as the launch image when the user taps (or slides) the action button (or slider).

Deprecated

