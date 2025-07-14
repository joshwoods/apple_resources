

- UIKit
- UILocalNotification
-  alertTitle Deprecated

Instance Property

# alertTitle

A short description of the reason for the alert.

iOS 8.2–10.0DeprecatediPadOS 8.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var alertTitle: String? { get set }
```

## Discussion

Use this property to provide a short description of the reason for the alert. You may specify a string with the text you want to display or you may specify a string to use as a lookup key in your app’s `Localizable.strings` file. The default value of this property is `nil`.

Title strings should be short, usually only a couple of words describing the reason for the notification. Apple Watch displays the title string as part of the short look notification interface, which has limited space.

## See Also

### Composing the alert

var alertBody: String?

The message displayed in the notification alert.

Deprecated

var alertAction: String?

The title of the action button or slider.

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

