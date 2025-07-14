

- UIKit
- UIUserNotificationSettings
-  init(types:categories:) Deprecated

Initializer

# init(types:categories:)

Creates and returns a settings object that you can use to register your requested notification and action types.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
convenience init(
    types: UIUserNotificationType,
    categories: Set?
)
```

## Parameters 

`types`  

The notification types that your app supports. For a list of possible values, see the constants for the UIUserNotificationType type.

`categories`  

A set of UIUserNotificationCategory objects that define the groups of actions a notification may include.

## Return Value

A new user notification settings object that you can register with the UIApplication object.

## Discussion

Use this method to create a new settings object that you intend to register with the app. When calling this method, specify the types of notifications you intend to deliver to the user such as alerts or sounds. If you intend to display custom actions in your notifications, use this method to register those actions as well.

After creating a new settings object, register that object by calling the registerUserNotificationSettings(_:) method of the shared UIApplication object.

