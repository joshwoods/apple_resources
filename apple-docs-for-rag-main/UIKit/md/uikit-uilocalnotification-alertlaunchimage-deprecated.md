

- UIKit
- UILocalNotification
-  alertLaunchImage Deprecated

Instance Property

# alertLaunchImage

Identifies the image used as the launch image when the user taps (or slides) the action button (or slider).

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var alertLaunchImage: String? { get set }
```

## Discussion

The string is a filename of an image file in the app bundle. This image is a launching image specified for a given notification; when the user taps the action button (for example, “View”) or moves the action slider, the image is used in place of the default launching image. If the value of this property is `nil` (the default), the system either uses the previous snapshot, uses the image identified by the `UILaunchImageFile` key in the app’s `Info.plist` file, or falls back to `Default.png`.

The value of this key has the exact same semantics as `UILaunchImageFile`. For more about this key, see the Information Property List Key Reference.

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

var category: String?

The name of a group of actions to display in the alert.

Deprecated

