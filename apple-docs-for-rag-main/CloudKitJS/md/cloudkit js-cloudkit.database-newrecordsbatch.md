

- CloudKit JS
- CloudKit.Database
-  newRecordsBatch 

Instance Method

# newRecordsBatch

Creates records batch builder object for modifying multiple records.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder newRecordsBatch(
 optional Object options
);
```

## Parameters 

`options`  

A dictionary containing options to use when modifying records. Possible dictionary keys are:

| Key | Description |
|----|----|
| `zoneID` | A CloudKit.ZoneID or zone name (`String`) that identifies the record zone in the database where you want to perform the operation. The default is the database default zone. |
| `desiredKeys` | An array of strings containing record field names that limits the amount of data returned in this operation. Only the fields specified in the array are returned. The default is `null`, which fetches all record fields. |
| `atomic` | A Boolean value indicating whether the entire operation fails when one or more operations fail.  If `true`, the entire request fails if one operation fails. If `false`, some operations may succeed and others may fail. The default value is `false`.  This property only applies to custom zones. |

## Return Value

A CloudKit.RecordsBatchBuilder object for this database.

## See Also

### Accessing Records

saveRecords

Saves records to the database.

fetchRecords

Fetches one or more records.

deleteRecords

Deletes one or more records.

performQuery

Fetches records by using a query.

