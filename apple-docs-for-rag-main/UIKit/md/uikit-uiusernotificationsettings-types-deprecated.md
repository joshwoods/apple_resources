

- UIKit
- UIUserNotificationSettings
-  types Deprecated

Instance Property

# types

A bitmask of the notification types that your app is allowed to use.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var types: UIUserNotificationType { get }
```

## Discussion

When you create a new settings object, this property contains all of the types you specified. After you register your request with the app, the app provides you with a new settings object that contains only the types that your app is allowed to use.

## See Also

### Related Documentation

class UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

Deprecated

### Getting the configured settings

var categories: Set&lt;UIUserNotificationCategory>?

The app’s registered groups of actions.

Deprecated

