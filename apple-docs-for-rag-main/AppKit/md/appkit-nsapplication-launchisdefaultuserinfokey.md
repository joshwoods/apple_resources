

- AppKit
- NSApplication
-  launchIsDefaultUserInfoKey 

Type Property

# launchIsDefaultUserInfoKey

The value for this key is an `NSNumber` containing a Boolean value. The value is false if the app was launched to open or print a file, to perform a Service action, if the app had saved state that will be restored, or if the app launch was in some other sense not a default launch. Otherwise its value will be true.

macOS 10.7+

``` source
class let launchIsDefaultUserInfoKey: String
```

## See Also

### Keys

class let launchUserNotificationUserInfoKey: String

A key that indicates your app was launched because a user activated a notification in the Notification Center.

