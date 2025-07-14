

- CloudKit JS
- CloudKit.Database
-  saveRecordZones 

Instance Method

# saveRecordZones

Creates one or more zones in the database.

CloudKit JS 1.0+

``` source
Promise saveRecordZones(
    CloudKit.ZoneID|CloudKit.ZoneID[]|String|String[] zones
);
```

## Parameters 

`zones`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.ZoneID | A zone in the database to save. |
| `CloudKit.ZoneID[]` | An array of zones to save. |
| `String` | The name of a zone to save. |
| `String[]` | An array of names of zones to save. |

## Return Value

A `Promise` object that resolves to a CloudKit.RecordZonesResponse object if the operation succeeds; otherwise, a CKError object.

## Discussion

See Modifying Zones (zones/modify) in CloudKit Web Services Reference.

## See Also

### Accessing Record Zones

fetchRecordZones

Fetches one or more zones.

fetchAllRecordZones

Fetches all zones in the database.

deleteRecordZones

Deletes the specified zones.

