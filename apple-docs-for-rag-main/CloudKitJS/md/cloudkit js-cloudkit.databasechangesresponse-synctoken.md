

- CloudKit JS
- CloudKit.DatabaseChangesResponse
-  syncToken 

Instance Property

# syncToken

A point in the database’s change history.

CloudKit JS 1.0+

``` source
readonly attribute String syncToken;
```

## Discussion

If moreComing is `true` in the response, use the this property in the next request until moreComing is `false`.

## See Also

### Response Properties

moreComing

A Boolean value that indicates there are more database changes to fetch.

zones

The zones in the database where the changes occurred.

