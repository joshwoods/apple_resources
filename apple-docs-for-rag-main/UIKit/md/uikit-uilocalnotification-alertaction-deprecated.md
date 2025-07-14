

- UIKit
- UILocalNotification
-  alertAction Deprecated

Instance Property

# alertAction

The title of the action button or slider.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var alertAction: String? { get set }
```

## Discussion

Assign a string or, preferably, a localized-string key (using NSLocalizedString) as the value. The alert action is the title of the right button of the alert or the value of the unlock slider, where the value replaces “unlock” in “slide to unlock”. If you specify `nil`, and alertBody is non-`nil`, “View” (localized to the preferred language) is used as the default value.

## See Also

### Composing the alert

var alertBody: String?

The message displayed in the notification alert.

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

