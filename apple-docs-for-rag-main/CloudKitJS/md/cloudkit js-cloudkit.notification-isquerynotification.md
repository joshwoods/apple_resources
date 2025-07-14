

- CloudKit JS
- CloudKit.Notification
-  isQueryNotification 

Instance Property

# isQueryNotification

A Boolean value indicating whether this push notification is a query notification.

CloudKit JS 1.0+

``` source
readonly attribute Boolean isQueryNotification;
```

## Discussion

`true` if this notification is a CloudKit.QueryNotification object; otherwise, `false`.

## See Also

### Getting the Notification Type

notificationType

The type of notification.

isRecordZoneNotification

A Boolean value indicating whether this notification is a push notification that was sent because of changes to a record zone.

