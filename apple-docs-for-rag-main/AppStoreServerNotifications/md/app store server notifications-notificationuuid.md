

- App Store Server Notifications
-  notificationUUID 

Type

# notificationUUID

A unique identifier for the notification.

App Store Server Notifications 2.0+

``` source
string notificationUUID
```

## Discussion

The App Store server assigns a unique identifer to each notification it sends. Use this value to identify, and ignore, duplicate notifications.

## See Also

### Response types

type notificationType

The type that describes the in-app purchase or external purchase event for which the App Store sends the version 2 notification.

type subtype

A string that provides details about select notification types in version 2.

type version

A string that indicates the notification’s App Store Server Notifications version number.

type signedDate

The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.

