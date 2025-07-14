

- AppKit
- NSApplication
-  launchUserNotificationUserInfoKey 

Type Property

# launchUserNotificationUserInfoKey

A key that indicates your app was launched because a user activated a notification in the Notification Center.

macOS 10.8+

``` source
class let launchUserNotificationUserInfoKey: String
```

## Discussion

The launchUserNotificationUserInfoKey key is an NSUserNotification object that is present in the userInfo dictionary of the didFinishLaunchingNotification notification if your app was launched because a user activated a notification in the Notification Center. To access the notification payload in the userInfo dictionary, you can use code like this:

```
NSUserNotification *userNotification = [[myNotification userInfo]
    objectForKey:NSApplicationLaunchUserNotificationKey];
    if (userNotification) {
        // The app was launched by a user selection from Notification Center.
    }
```

## See Also

### Keys

class let launchIsDefaultUserInfoKey: String

The value for this key is an `NSNumber` containing a Boolean value. The value is false if the app was launched to open or print a file, to perform a Service action, if the app had saved state that will be restored, or if the app launch was in some other sense not a default launch. Otherwise its value will be true.

