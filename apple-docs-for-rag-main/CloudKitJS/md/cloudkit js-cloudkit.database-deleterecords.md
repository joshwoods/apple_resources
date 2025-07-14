

- CloudKit JS
- CloudKit.Database
-  deleteRecords 

Instance Method

# deleteRecords

Deletes one or more records.

CloudKit JS 1.0+

``` source
Promise deleteRecords(
    CloudKit.Record|CloudKit.Record[]|String|String[] records,
 optional Object options
);
```

## Parameters 

`records`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.Record | A dictionary or the record name of the record to delete. |
| `CloudKit.Record[]` | An array of records to delete. |
| `String` | The name of a record to delete. |
| `String[]` | An array of names of records to delete. |

`options`  

A dictionary containing a single `zoneID` key that identifies the zone (CloudKit.ZoneID) in the database where the record resides. If the `options` parameter is omitted, the default zone is used.

## Return Value

A `Promise` object that resolves to a CloudKit.RecordsResponse object if the operation succeeds; otherwise, a CKError object.

## See Also

### Accessing Records

saveRecords

Saves records to the database.

fetchRecords

Fetches one or more records.

performQuery

Fetches records by using a query.

newRecordsBatch

Creates records batch builder object for modifying multiple records.

