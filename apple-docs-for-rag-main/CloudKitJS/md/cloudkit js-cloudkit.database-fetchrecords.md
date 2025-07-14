

- CloudKit JS
- CloudKit.Database
-  fetchRecords 

Instance Method

# fetchRecords

Fetches one or more records.

CloudKit JS 1.0+

``` source
Promise fetchRecords(
    CloudKit.Record|CloudKit.Record[]|String|String[] records,
 optional Object options
);
```

## Parameters 

`records`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.Record | A dictionary record to fetch. Only the `recordName` key is required in the CloudKit.Record dictionary. |
| `CloudKit.Record[]` | An array of records to fetch. |
| `String` | The name of a record to fetch. |
| `String[]` | An array of names of records to fetch. |

`options`  

A dictionary containing options to use when fetching records. Possible dictionary keys are:

| Key | Description |
|----|----|
| `zoneID` | A CloudKit.ZoneID or zone name (`String`) that identifies the record zone in the database where you want to perform the operation. The default is the database default zone. |
| `desiredKeys` | An array of strings containing record field names that limits the amount of data returned in this operation. Only the fields specified in the array are returned. The default is `null`, which fetches all record fields. |
| `numbersAsStrings` | A Boolean value indicating whether number fields should be represented by strings. The default value is `false`. |

## Return Value

A `Promise` object that resolves to a CloudKit.RecordsResponse object if the operation succeeds; otherwise, a CKError object.

## Discussion

To get the fetched record, use the records property in the CloudKit.RecordsResponse class.

```
database.fetchRecords('115').then(function(response) {
    if (response.hasErrors) {
        // Insert error handling
        throw response.errors[0];
    } else {
        // Insert successfully fetched record
        var fetchedRecord = response.records[0];
    }
});
```

Similar to the saveRecords method, if you don’t specify a zone ID in the `options` parameter, the records are fetched from the default zone. To fetch records from a specific zone, pass a dictionary with the `zoneID` key set to the name of your zone.

```
database.fetchRecords('115', { zoneID: 'myZone' }).then(function(response) {
    // …
}
```

## See Also

### Accessing Records

saveRecords

Saves records to the database.

deleteRecords

Deletes one or more records.

performQuery

Fetches records by using a query.

newRecordsBatch

Creates records batch builder object for modifying multiple records.

