

- User Notifications
- UNUserNotificationCenter
-  getNotificationSettings(completionHandler:) 

Instance Method

# getNotificationSettings(completionHandler:)

Retrieves the authorization and feature-related settings for your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func getNotificationSettings(completionHandler: @escaping (UNNotificationSettings) -> Void)
```

``` source
func notificationSettings() async -> UNNotificationSettings
```

## Parameters 

`completionHandler`  

The block to execute asynchronously with the results. Your app may execute this block on a background thread. The block has no return value and takes the following parameter:

settings  
The UNNotificationSettings object containing the current authorization settings for your app.

## Mentioned in 

Asking permission to use notifications

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func notificationSettings() async -> UNNotificationSettings
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to determine the user interactions and notification-related features that the system authorizes your app to use. You might then use this information to enable or disable specific notification-related features of your app.

```
let center = UNUserNotificationCenter.current()
let settings = await center.notificationSettings()
// Add code here to inspect or act on the settings.
```

When the user initially grants authorization to your app, the system gives your app a set of default notification-related settings. The user may change those settings at any time to enable or disable specific capabilities. For example, the user might disable the playing of sounds when a notification arrives.

## See Also

### Managing the notification center

class func current() -> UNUserNotificationCenter

Returns your app’s notification center.

func setBadgeCount(Int, withCompletionHandler: (((any Error)?) -> Void)?)

Updates the badge count for your app’s icon.

