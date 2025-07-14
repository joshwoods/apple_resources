

- UIKit
- UILocalNotification
-  hasAction Deprecated

Instance Property

# hasAction

A Boolean value that controls whether the notification shows or hides the alert action.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var hasAction: Bool { get set }
```

## Discussion

Assign false to this property to hide the alert button or slider. (This effect requires alertBody to be non-`nil`.) The default value is true.

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

var alertLaunchImage: String?

Identifies the image used as the launch image when the user taps (or slides) the action button (or slider).

Deprecated

var category: String?

The name of a group of actions to display in the alert.

Deprecated

