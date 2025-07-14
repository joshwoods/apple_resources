

- CloudKit JS
- CloudKit.Database
-  deleteRecordZones 

Instance Method

# deleteRecordZones

Deletes the specified zones.

CloudKit JS 1.0+

``` source
Promise deleteRecordZones(
    CloudKit.ZoneID|CloudKit.ZoneID[]|String|String[] zones
);
```

## Parameters 

`zones`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.ZoneID | A zone in the database to delete. |
| `CloudKit.ZoneID[]` | An array of zones to delete. |
| `String` | The name of a zone to delete. |
| `String[]` | An array of names of zones to delete. |

## Return Value

A `Promise` object that resolves to a CloudKit.RecordZonesResponse object if the operation succeeds; otherwise, a CKError object.

## See Also

### Accessing Record Zones

saveRecordZones

Creates one or more zones in the database.

fetchRecordZones

Fetches one or more zones.

fetchAllRecordZones

Fetches all zones in the database.

