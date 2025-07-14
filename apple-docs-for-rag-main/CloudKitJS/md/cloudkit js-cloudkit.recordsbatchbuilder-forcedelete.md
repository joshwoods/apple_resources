

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  forceDelete 

Instance Method

# forceDelete

Deletes one or more records regardless of conflicts.

CloudKit JS 1.0+

``` source
RecordsBatchBuilder forceDelete(
    CloudKit.Record|CloudKit.Record[] records
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the record to delete, if you are deleting a single record. If you are deleting multiple records, this parameter is an array of CloudKit.Record dictionaries. The `recordChangeTag` key is not required in the CloudKit.Record dictionaries.

## Return Value

The object that received this method call.

## See Also

### Deleting Records

delete

Deletes one or more records.

