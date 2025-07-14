

- UIKit
- UILocalNotification
-  userInfo Deprecated

Instance Property

# userInfo

A dictionary for passing custom information to the notified app.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

You may add arbitrary key-value pairs to this dictionary. However, the keys and values must be valid Property list; if any are not, an exception is raised.

## See Also

### Configuring other parts of the notification

var applicationIconBadgeNumber: Int

The number to display as the app’s icon badge.

Deprecated

var soundName: String?

The name of the file containing the sound to play when an alert is displayed.

Deprecated

