

- CloudKit JS
- CloudKit.QueryNotification
-  queryNotificationReason 

Instance Property

# queryNotificationReason

The reason for the query notification.

CloudKit JS 1.0+

``` source
readonly attribute String queryNotificationReason;
```

## Discussion

Possible values are described in Reasons for Query Notifications.

## See Also

### Getting Record Changes

recordName

The name of the record that was created, deleted, or updated.

recordFields

A dictionary representation of the fields that changed in the record.

isPublicDatabase

Boolean value indicating whether the notification is from the public database.

