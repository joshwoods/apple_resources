

- UIKit
- UIUserNotificationSettings
-  categories Deprecated

Instance Property

# categories

The app’s registered groups of actions.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var categories: Set? { get }
```

## Discussion

This property contains the UIUserNotificationCategory objects that you specified when creating the settings object. Each object corresponds to a group of actions that may be displayed in conjunction with a push notification. After registration, this property contains the set of actions you specified in your initial request.

## See Also

### Related Documentation

convenience init(types: UIUserNotificationType, categories: Set&lt;UIUserNotificationCategory>?)

Creates and returns a settings object that you can use to register your requested notification and action types.

Deprecated

### Getting the configured settings

var types: UIUserNotificationType

A bitmask of the notification types that your app is allowed to use.

Deprecated

