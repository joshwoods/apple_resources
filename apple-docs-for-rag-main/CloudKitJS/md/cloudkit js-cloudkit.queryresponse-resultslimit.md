

- CloudKit JS
- CloudKit.QueryResponse
-  resultsLimit 

Instance Property

# resultsLimit

The maximum number of records to fetch.

CloudKit JS 1.0+

``` source
readonly attribute Number resultsLimit;
```

## Discussion

The default is the maximum number of records in a response that is allowed, described in Data Size Limits in CloudKit Web Services Reference.

## See Also

### Related Documentation

moreComing

A Boolean value that indicates whether there are more records to fetch.

### Accessing Request Properties

zoneID

A CloudKit.ZoneID dictionary that identifies a record zone in the database.

continuationMarker

Marks the location of the last batch of results.

desiredKeys

An array of strings containing record field names that limits the amount of data returned in this operation.

zoneWide

A Boolean value that determines whether all zones should be searched.

