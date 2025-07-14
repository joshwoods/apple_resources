

- UIKit
- UIMutableUserNotificationCategory
-  setActions(\_:for:) Deprecated

Instance Method

# setActions(\_:for:)

Sets the actions to display for different alert styles.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setActions(
    _ actions: [UIUserNotificationAction]?,
    for context: UIUserNotificationActionContext
)
```

## Parameters 

`actions`  

An array of UIUserNotificationAction objects representing the actions to display for the given context. When displaying the notification to the user, the system displays the action buttons using the same order as the items in this array. If you specify `nil` or an empty array, this method removes the actions for the specified context.

`context`  

The context in which the alert is displayed. For a list of possible values, see UIUserNotificationActionContext.

## Discussion

Use this method to set or change the actions associated with a specific context.

## See Also

### Modifying the action settings

var identifier: String?

The name of the action group.

Deprecated

