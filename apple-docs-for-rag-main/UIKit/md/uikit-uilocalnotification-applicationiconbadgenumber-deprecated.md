

- UIKit
- UILocalNotification
-  applicationIconBadgeNumber Deprecated

Instance Property

# applicationIconBadgeNumber

The number to display as the app’s icon badge.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var applicationIconBadgeNumber: Int { get set }
```

## Discussion

The default value of this property is 0, which means that no badge is displayed.

## See Also

### Configuring other parts of the notification

var soundName: String?

The name of the file containing the sound to play when an alert is displayed.

Deprecated

var userInfo: [AnyHashable : Any]?

A dictionary for passing custom information to the notified app.

Deprecated

