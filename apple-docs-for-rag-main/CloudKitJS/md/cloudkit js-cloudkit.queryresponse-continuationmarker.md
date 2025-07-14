

- CloudKit JS
- CloudKit.QueryResponse
-  continuationMarker 

Instance Property

# continuationMarker

Marks the location of the last batch of results.

CloudKit JS 1.0+

``` source
readonly attribute String continuationMarker;
```

## Discussion

Pass this key to another performQuery method call when the results of a previous fetch exceed the maximum.

## See Also

### Related Documentation

moreComing

A Boolean value that indicates whether there are more records to fetch.

### Accessing Request Properties

zoneID

A CloudKit.ZoneID dictionary that identifies a record zone in the database.

resultsLimit

The maximum number of records to fetch.

desiredKeys

An array of strings containing record field names that limits the amount of data returned in this operation.

zoneWide

A Boolean value that determines whether all zones should be searched.

