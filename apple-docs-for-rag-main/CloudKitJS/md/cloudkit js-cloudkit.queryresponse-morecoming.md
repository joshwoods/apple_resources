

- CloudKit JS
- CloudKit.QueryResponse
-  moreComing 

Instance Property

# moreComing

A Boolean value that indicates whether there are more records to fetch.

CloudKit JS 1.0+

``` source
readonly attribute Boolean moreComing;
```

## Discussion

This property is `true` if there are more records to fetch; otherwise, `false`. If the number of records matching the query exceeds the number of records allowed in a single response, this property is `true` until all the records are returned.

## See Also

### Related Documentation

continuationMarker

Marks the location of the last batch of results.

resultsLimit

The maximum number of records to fetch.

### Accessing Response Properties

query

A CloudKit.Query dictionary containing the criteria for matching records in the database.

