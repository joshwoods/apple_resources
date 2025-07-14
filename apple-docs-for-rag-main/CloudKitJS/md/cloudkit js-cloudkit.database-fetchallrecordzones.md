

- CloudKit JS
- CloudKit.Database
-  fetchAllRecordZones 

Instance Method

# fetchAllRecordZones

Fetches all zones in the database.

CloudKit JS 1.0+

``` source
Promise fetchAllRecordZones();
```

## Return Value

A `Promise` object that resolves to a CloudKit.RecordZonesResponse object or if it fails, a CKError object.

## Discussion

See Fetching Zones (zones/list) in CloudKit Web Services Reference.

## See Also

### Accessing Record Zones

saveRecordZones

Creates one or more zones in the database.

fetchRecordZones

Fetches one or more zones.

deleteRecordZones

Deletes the specified zones.

