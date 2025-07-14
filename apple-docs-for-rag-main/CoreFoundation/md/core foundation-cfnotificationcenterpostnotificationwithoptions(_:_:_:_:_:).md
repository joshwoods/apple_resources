

- Core Foundation
-  CFNotificationCenterPostNotificationWithOptions(\_:\_:\_:\_:\_:) 

Function

# CFNotificationCenterPostNotificationWithOptions(\_:\_:\_:\_:\_:)

Posts a notification for an object using specified options.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterPostNotificationWithOptions(
    _ center: CFNotificationCenter!,
    _ name: CFNotificationName!,
    _ object: UnsafeRawPointer!,
    _ userInfo: CFDictionary!,
    _ options: CFOptionFlags
)
```

## Parameters 

`center`  

The notification center to post the notification.

`name`  

The name of the notification to post. This value must not be `NULL`.

`object`  

The object posting the notification. If `NULL`, the notification is sent only to observers that are observing all objects. In other words, only observers that registered for the notification with a `NULL` value for `object` will receive the notification.

If you want to allow your clients to register for notifications using Cocoa APIs (see NotificationCenter), then `object` must be a Core Foundation or Cocoa object.

For distributed notifications, `object` must be a CFString object.

If `center` is a Darwin notification center, this value is ignored.

`userInfo`  

A dictionary to pass to observers. You populate this dictionary with additional information describing the notification. For distributed notifications, the dictionary must contain only property list objects. Can be `NULL`. If `center` is a Darwin notification center, this value is ignored.

`options`  

Specifies if the notification should be posted immediately, or to all sessions. See Notification Posting Options for possible values.

If `center` is a Darwin notification center, this value is ignored.

## See Also

### Posting a Notification

func CFNotificationCenterPostNotification(CFNotificationCenter!, CFNotificationName!, UnsafeRawPointer!, CFDictionary!, Bool)

Posts a notification for an object.

