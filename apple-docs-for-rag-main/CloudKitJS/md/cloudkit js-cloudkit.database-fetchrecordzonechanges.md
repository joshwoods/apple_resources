

- CloudKit JS
- CloudKit.Database
-  fetchRecordZoneChanges 

Instance Method

# fetchRecordZoneChanges

Fetch changes to the specified record zones in the database.

CloudKit JS 1.0+

``` source
Promise fetchRecordZoneChanges(
    CloudKit.RecordZoneChangesOptions|CloudKit.RecordZoneChangesOptions[] options
);
```

## Parameters 

`options`  

Specifies the zones and what data to fetch from each. If you want to fetch from multiple zones, pass an array containing a CloudKit.RecordZoneChangesOptions dictionary for each zone.

## Return Value

A `Promise` object that resolves to a CloudKit.RecordZoneChangesResponse object, or rejects to a CKError object.

## Discussion

Use the fetchDatabaseChanges method to get the zones that contain changed records.

## See Also

### Fetching Changes

databaseScope

The type of database (public, private, or shared).

fetchDatabaseChanges

Fetch changed record zones in the database.

