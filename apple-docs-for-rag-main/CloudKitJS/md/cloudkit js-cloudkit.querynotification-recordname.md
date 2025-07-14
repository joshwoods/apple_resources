

- CloudKit JS
- CloudKit.QueryNotification
-  recordName 

Instance Property

# recordName

The name of the record that was created, deleted, or updated.

CloudKit JS 1.0+

``` source
readonly attribute String recordName;
```

## See Also

### Getting Record Changes

queryNotificationReason

The reason for the query notification.

recordFields

A dictionary representation of the fields that changed in the record.

isPublicDatabase

Boolean value indicating whether the notification is from the public database.

