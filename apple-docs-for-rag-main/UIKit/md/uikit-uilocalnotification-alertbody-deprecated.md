

- UIKit
- UILocalNotification
-  alertBody Deprecated

Instance Property

# alertBody

The message displayed in the notification alert.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var alertBody: String? { get set }
```

## Discussion

Assign a string or, preferably, a localized-string key (using NSLocalizedString) as the value of the message. If the value of this property is non-`nil`, an alert is displayed. The default value is `nil` (no alert). Printf style escape characters are stripped from the string prior to display; to include a percent symbol (%) in the message, use two percent symbols (%%).

## See Also

### Composing the alert

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

var category: String?

The name of a group of actions to display in the alert.

Deprecated

