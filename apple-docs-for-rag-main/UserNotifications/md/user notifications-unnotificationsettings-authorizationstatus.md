

- User Notifications
- UNNotificationSettings
-  authorizationStatus 

Instance Property

# authorizationStatus

The app’s ability to schedule and receive local and remote notifications.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var authorizationStatus: UNAuthorizationStatus { get }
```

## Discussion

When the value of this property is UNAuthorizationStatus.authorized, your app is allowed to schedule and receive local and remote notifications. When authorized, use the alertSetting, badgeSetting, and soundSetting properties to specify which types of interactions are allowed. When the value of the property is UNAuthorizationStatus.denied, the system doesn’t deliver notifications to your app, and the system ignores any attempts to schedule local notifications.

The value of this property is UNAuthorizationStatus.notDetermined if your app has never requested authorization using the requestAuthorization(options:completionHandler:) method.

## See Also

### Getting the Authorization Status

enum UNAuthorizationStatus

Constants indicating whether the app is allowed to schedule notifications.

