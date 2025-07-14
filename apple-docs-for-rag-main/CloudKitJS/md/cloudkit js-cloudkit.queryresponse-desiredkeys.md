

- CloudKit JS
- CloudKit.QueryResponse
-  desiredKeys 

Instance Property

# desiredKeys

An array of strings containing record field names that limits the amount of data returned in this operation.

CloudKit JS 1.0+

``` source
readonly attribute String[] desiredKeys;
```

## Discussion

The default is `null`, which fetches all record fields.

## See Also

### Accessing Request Properties

zoneID

A CloudKit.ZoneID dictionary that identifies a record zone in the database.

resultsLimit

The maximum number of records to fetch.

continuationMarker

Marks the location of the last batch of results.

zoneWide

A Boolean value that determines whether all zones should be searched.

