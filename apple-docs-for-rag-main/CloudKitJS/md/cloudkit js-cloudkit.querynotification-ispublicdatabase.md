

- CloudKit JS
- CloudKit.QueryNotification
-  isPublicDatabase 

Instance Property

# isPublicDatabase

Boolean value indicating whether the notification is from the public database.

CloudKit JS 1.0+

``` source
readonly attribute Boolean isPublicDatabase;
```

## Discussion

`true` if the notification is from the public database; otherwise, `false`.

## See Also

### Getting Record Changes

queryNotificationReason

The reason for the query notification.

recordName

The name of the record that was created, deleted, or updated.

recordFields

A dictionary representation of the fields that changed in the record.

