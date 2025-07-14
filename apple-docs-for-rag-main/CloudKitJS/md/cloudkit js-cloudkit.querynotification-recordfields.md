

- CloudKit JS
- CloudKit.QueryNotification
-  recordFields 

Instance Property

# recordFields

A dictionary representation of the fields that changed in the record.

CloudKit JS 1.0+

``` source
readonly attribute Object recordFields;
```

## Discussion

The keys are the record field names, and the values are the record field values.

## See Also

### Getting Record Changes

queryNotificationReason

The reason for the query notification.

recordName

The name of the record that was created, deleted, or updated.

isPublicDatabase

Boolean value indicating whether the notification is from the public database.

