

- User Notifications
- UNUserNotificationCenter
-  current() 

Type Method

# current()

Returns your app’s notification center.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class func current() -> UNUserNotificationCenter
```

## Return Value

The notification center object to use.

## Discussion

Always use this method to retrieve the shared notification center object for your app. Do not try to create instances of the UNUserNotificationCenter class directly.

## See Also

### Managing the notification center

func getNotificationSettings(completionHandler: (UNNotificationSettings) -> Void)

Retrieves the authorization and feature-related settings for your app.

func setBadgeCount(Int, withCompletionHandler: (((any Error)?) -> Void)?)

Updates the badge count for your app’s icon.

