

- CloudKit JS
- CloudKit.RecordZonesResponse
-  zones 

Instance Property

# zones

The zones for the successful database operations.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.RecordZone[] zones;
```

## Discussion

The objects in the array have a single property with this format: `{zoneID: {zoneName: ‘zone’}}`.

