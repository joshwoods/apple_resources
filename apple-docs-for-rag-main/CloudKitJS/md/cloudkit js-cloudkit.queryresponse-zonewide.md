

- CloudKit JS
- CloudKit.QueryResponse
-  zoneWide 

Instance Property

# zoneWide

A Boolean value that determines whether all zones should be searched.

CloudKit JS 1.0+

``` source
readonly attribute Boolean zoneWide;
```

## Discussion

If `true`, all zones are searched. If `false`, only the default zone is searched.

## See Also

### Accessing Request Properties

zoneID

A CloudKit.ZoneID dictionary that identifies a record zone in the database.

resultsLimit

The maximum number of records to fetch.

continuationMarker

Marks the location of the last batch of results.

desiredKeys

An array of strings containing record field names that limits the amount of data returned in this operation.

