

- CloudKit JS
- CloudKit.Database
-  fetchRecordZones 

Instance Method

# fetchRecordZones

Fetches one or more zones.

CloudKit JS 1.0+

``` source
Promise fetchRecordZones(
    CloudKit.ZoneID|CloudKit.ZoneID[]|String|String[] zones
);
```

## Parameters 

`zones`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.ZoneID | A zone in the database to fetch. |
| `CloudKit.ZoneID[]` | An array of zones to fetch. |
| `String` | The name of a zone to fetch. |
| `String[]` | An array of names of zones to fetch. |

## Return Value

A `Promise` object that resolves to a CloudKit.RecordZonesResponse object if the operation succeeds; otherwise, a CKError object.

## Discussion

See Fetching Zones by Identifier (zones/lookup) in CloudKit Web Services Reference.

## See Also

### Accessing Record Zones

saveRecordZones

Creates one or more zones in the database.

fetchAllRecordZones

Fetches all zones in the database.

deleteRecordZones

Deletes the specified zones.

