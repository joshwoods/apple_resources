

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  update 

Instance Method

# update

Updates one or more existing records.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder update(
    CloudKit.Record|CloudKit.Record[] records,
 optional Object options
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the fields of the record you want to update, if you are updating a single record. If you are updating multiple records, this parameter is an array of CloudKit.Record dictionaries. The CloudKit.Record dictionaries need to contain the `recordChangeTag` key. Only the values of the fields in these dictionaries are updated.

`options`  

A dictionary containing options for this operation. This parameter contains a single `desiredKeys` key that is an array of field names (`String` values). Only the fields specified in the array are set.

## Return Value

The object that received this method call.

## See Also

### Creating and Updating Records

create

Creates one or more records.

createOrUpdate

Creates or updates one or more records depending on the information provided.

forceUpdate

Updates one or more existing records regardless of conflicts.

