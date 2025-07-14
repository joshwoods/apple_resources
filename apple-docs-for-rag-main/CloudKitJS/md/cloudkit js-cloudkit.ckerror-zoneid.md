

- CloudKit JS
- CloudKit.CKError
-  zoneID 

Instance Property

# zoneID

The record zone in the database where the error occurred.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.ZoneID zoneID;
```

## Discussion

This property value is `Undefined` if the error is unrelated to a zone operation.

## See Also

### Identifying the Operation

recordName

The name of the record that the operation failed on.

subscriptionID

A string that is a unique identifier for the subscription where the error occurred.

