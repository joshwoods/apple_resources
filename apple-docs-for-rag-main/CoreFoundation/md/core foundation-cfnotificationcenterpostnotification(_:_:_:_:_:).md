

- Core Foundation
-  CFNotificationCenterPostNotification(\_:\_:\_:\_:\_:) 

Function

# CFNotificationCenterPostNotification(\_:\_:\_:\_:\_:)

Posts a notification for an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNotificationCenterPostNotification(
    _ center: CFNotificationCenter!,
    _ name: CFNotificationName!,
    _ object: UnsafeRawPointer!,
    _ userInfo: CFDictionary!,
    _ deliverImmediately: Bool
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

A dictionary passed to observers. You populate this dictionary with additional information describing the notification. For distributed notifications, the dictionary must contain only property list objects. This value may be `NULL`.

If `center` is a Darwin notification center, this value is ignored.

`deliverImmediately`  

If `true`, the notification is delivered to all observers immediately, even if some observers are in suspended (background) applications and they requested different suspension behavior when registering for the notification. If `false`, each observer’s requested suspension behavior is respected.

If `center` is a Darwin notification center, this value is ignored.

## See Also

### Posting a Notification

func CFNotificationCenterPostNotificationWithOptions(CFNotificationCenter!, CFNotificationName!, UnsafeRawPointer!, CFDictionary!, CFOptionFlags)

Posts a notification for an object using specified options.

