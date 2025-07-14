

- UIKit
- UIMutableUserNotificationAction
-  identifier Deprecated

Instance Property

# identifier

The string that you use internally to identify the action.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var identifier: String? { get set }
```

## Discussion

The system passes this string to the application(_:handleActionWithIdentifier:for:completionHandler:) or application(_:handleActionWithIdentifier:forRemoteNotification:completionHandler:) method of the app delegate when the user chooses the action.

## See Also

### Getting the action information

var title: String?

The localized string to use as the button title for the action.

Deprecated

