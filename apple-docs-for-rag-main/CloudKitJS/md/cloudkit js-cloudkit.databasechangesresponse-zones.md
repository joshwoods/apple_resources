

- CloudKit JS
- CloudKit.DatabaseChangesResponse
-  zones 

Instance Property

# zones

The zones in the database where the changes occurred.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.RecordZoneChangesOptions[] zones;
```

## Discussion

To fetch record changes in these zones, pass this property to the fetchRecordZoneChanges method in the CloudKit.Database class.

## See Also

### Response Properties

moreComing

A Boolean value that indicates there are more database changes to fetch.

syncToken

A point in the database’s change history.

