

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  createOrUpdate 

Instance Method

# createOrUpdate

Creates or updates one or more records depending on the information provided.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder createOrUpdate(
    CloudKit.Record|CloudKit.Record[] records,
 optional Object options
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the record to create or update, if you are updating a single record. If you are updating multiple records, this parameter is an array of CloudKit.Record dictionaries representing the records to create or update. Only the values of the fields in the dictionaries are set.

`options`  

A dictionary containing options for this operation. This parameter contains a single `desiredKeys` key that is an array of field names (`String` values). Only the fields specified in the array are set.

## Return Value

The object that received this method call.

## Discussion

This is a convenience method for adding create and update operations rather than adding them separately using the create and update methods. Depending on the information in the record, this method determines whether the record should be created or updated.

The type of operation depends on the values of the `recordName` and `recordChangeTag` keys in the CloudKit.Record dictionaries.

- To create a record with a server-generated record name, set the `recordName` and `recordChangeTag` keys to `null`.

- To create a record with a specified record name, set the `recordName` key to the record name and set `recordChangeTag` to `null`.

- To update an existing record, set the `recordName` and `recordChangeTag` keys to non-`null` values.

An error occurs if the `recordName` key is `null` and the `recordChangeTag` key is non-`null`. Retain the record name of records you previously fetched, and include it when updating a record.

## See Also

### Creating and Updating Records

create

Creates one or more records.

update

Updates one or more existing records.

forceUpdate

Updates one or more existing records regardless of conflicts.

