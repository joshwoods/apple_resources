

- User Notifications
- UNUserNotificationCenterDelegate
-  userNotificationCenter(\_:willPresent:withCompletionHandler:) 

Instance Method

# userNotificationCenter(\_:willPresent:withCompletionHandler:)

Asks the delegate how to handle a notification that arrived while the app was running in the foreground.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
optional func userNotificationCenter(
    _ center: UNUserNotificationCenter,
    willPresent notification: UNNotification,
    withCompletionHandler completionHandler: @escaping (UNNotificationPresentationOptions) -> Void
)
```

``` source
optional func userNotificationCenter(
    _ center: UNUserNotificationCenter,
    willPresent notification: UNNotification
) async -> UNNotificationPresentationOptions
```

## Parameters 

`center`  

The shared user notification center object that received the notification.

`notification`  

The notification that is about to be delivered. Use the information in this object to determine an appropriate course of action. For example, you might use the information to update your app’s interface.

`completionHandler`  

The block to execute with the presentation option for the notification. Always execute this block at some point during your implementation of this method. Use the `options` parameter to specify how you want the system to alert the user, if at all. This block has no return value and takes the following parameter:

options  
The option for notifying the user. Specify UNNotificationPresentationOptionNone to silence the notification completely. Specify other values to interact with the user. For a list of possible options, see UNNotificationPresentationOptions.

## Mentioned in 

Asking permission to use notifications

Handling notifications and notification-related actions

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func userNotificationCenter(_ center: UNUserNotificationCenter, willPresent notification: UNNotification) async -> UNNotificationPresentationOptions
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If your app is in the foreground when a notification arrives, the shared user notification center calls this method to deliver the notification directly to your app. If you implement this method, you can take whatever actions are necessary to process the notification and update your app. When you finish, call the `completionHandler` block and specify how you want the system to alert the user, if at all.

If your delegate does not implement this method, the system behaves as if you had passed the UNNotificationPresentationOptionNone option to the `completionHandler` block. If you do not provide a delegate at all for the UNUserNotificationCenter object, the system uses the notification’s original options to alert the user.

## See Also

### Receiving Notifications

struct UNNotificationPresentationOptions

Constants indicating how to present a notification in a foreground app.

