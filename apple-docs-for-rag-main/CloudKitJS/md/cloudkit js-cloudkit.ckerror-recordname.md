

- CloudKit JS
- CloudKit.CKError
-  recordName 

Instance Property

# recordName

The name of the record that the operation failed on.

CloudKit JS 1.0+

``` source
readonly attribute String recordName;
```

## Discussion

This property value is `Undefined` if the error is unrelated to a record operation.

## See Also

### Identifying the Operation

subscriptionID

A string that is a unique identifier for the subscription where the error occurred.

zoneID

The record zone in the database where the error occurred.

