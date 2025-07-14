

- App Store Server Notifications
-  version 

Type

# version

A string that indicates the notification’s App Store Server Notifications version number.

App Store Server Notifications 2.5+

``` source
string version
```

## Discussion

The version string is `“2.0”`. It’s present in responseBodyV2DecodedPayload for version 2 notifications.

For more information about App Store Server Notification changes, see App Store Server Notifications changelog.

## See Also

### Response types

type notificationType

The type that describes the in-app purchase or external purchase event for which the App Store sends the version 2 notification.

type subtype

A string that provides details about select notification types in version 2.

type signedDate

The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.

type notificationUUID

A unique identifier for the notification.

