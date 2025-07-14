

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  create 

Instance Method

# create

Creates one or more records.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder create(
    CloudKit.Record|CloudKit.Record[] records,
 optional Object options
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the record to create, if you are creating a single record. If you are creating multiple records, this parameter is an array of CloudKit.Record dictionaries representing the records to create. Only the values of the fields in the dictionaries are set.

`options`  

A dictionary containing options for this operation. This parameter contains a single `desiredKeys` key that is an array of field names (`String` values). Only the fields specified in the array are set.

## Return Value

The object that received this method call.

## See Also

### Creating and Updating Records

createOrUpdate

Creates or updates one or more records depending on the information provided.

update

Updates one or more existing records.

forceUpdate

Updates one or more existing records regardless of conflicts.

