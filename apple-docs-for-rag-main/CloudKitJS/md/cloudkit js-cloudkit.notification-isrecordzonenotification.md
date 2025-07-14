

- CloudKit JS
- CloudKit.Notification
-  isRecordZoneNotification 

Instance Property

# isRecordZoneNotification

A Boolean value indicating whether this notification is a push notification that was sent because of changes to a record zone.

CloudKit JS 1.0+

``` source
readonly attribute Boolean isRecordZoneNotification;
```

## Discussion

`true` if this notification is a CloudKit.RecordZoneNotification object; otherwise, `false`.

## See Also

### Getting the Notification Type

notificationType

The type of notification.

isQueryNotification

A Boolean value indicating whether this push notification is a query notification.

