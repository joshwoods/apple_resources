

- AppKit
- NSApplicationDelegate
-  application(\_:didReceiveRemoteNotification:) 

Instance Method

# application(\_:didReceiveRemoteNotification:)

Tells the delegate when the app receives a remote notification.

macOS 10.7+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    didReceiveRemoteNotification userInfo: [String : Any]
)
```

## Parameters 

`application`  

The application that received the remote notification.

`userInfo`  

A dictionary that contains information related to the remote notification, specifically a badge number for the application icon, a notification identifier, and possibly custom data. The provider originates it as a JSON-defined dictionary that AppKit converts to an NSDictionary object; the dictionary may contain only property-list objects plus NSNull.

## Discussion

The delegate receives this message when the application is running and a remote notification arrives for it. In response, the application typically connects with its provider and downloads the data waiting for it. It may also process the notification in any other way it deems useful.

The `userInfo` dictionary contains another dictionary that you can obtain using the `aps` key. You can access the contents of the `aps` dictionary using the following keys:

- `badge`—A number indicating the quantity of data items to obtain from the provider. This number is to be displayed on the application icon. The absence of a `badge` property indicates that any number currently badging the icon should be removed.

Icon badging is the only notification type supported for non-running applications.

- `alert`—The value may either be a string for the alert message or a dictionary with two keys: `body` and `show-view`. The value of the former is the alert message and the latter is a Boolean (`false` or `true`). You may ignore the second key.

- `sound`—The name of a sound file in the application bundle to play as an alert sound. If “default” is specified, the default sound should be played.

The `userInfo` dictionary may also have custom data defined by the provider according to the JSON schema. The properties for custom data should be specified at the same level as the `aps` dictionary. However, custom-defined properties should not be used for mass data transport because there is a strict size limit per notification (256 bytes) and delivery is not guaranteed.

If you implement applicationDidFinishLaunching(_:) and a push notification for the application has recently arrived, this method is not invoked for that push notification. In this case, you can access the JSON data in the userInfo dictionary of the passed-in NSNotification object.

For more information about how to implement push notifications in your application, see Local and Remote Notification Programming Guide.

## See Also

### Handling Push Notifications

func application(NSApplication, didRegisterForRemoteNotificationsWithDeviceToken: Data)

Tells the delegate that the app registered for Apple Push Services.

func application(NSApplication, didFailToRegisterForRemoteNotificationsWithError: any Error)

Tells the delegate that the app was unable to register for Apple Push Services.

