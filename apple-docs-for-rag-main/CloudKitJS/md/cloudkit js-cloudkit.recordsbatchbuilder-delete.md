

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  delete 

Instance Method

# delete

Deletes one or more records.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder delete(
    CloudKit.Record|CloudKit.Record[] records
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the record to delete, if you are deleting a single record. If you are deleting multiple records, this parameter is an array of CloudKit.Record dictionaries. The CloudKit.Record dictionaries need to contain the `recordChangeTag` key.

## Return Value

The object that received this method call.

## See Also

### Deleting Records

forceDelete

Deletes one or more records regardless of conflicts.

