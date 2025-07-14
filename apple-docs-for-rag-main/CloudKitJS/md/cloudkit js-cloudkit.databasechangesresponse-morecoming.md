

- CloudKit JS
- CloudKit.DatabaseChangesResponse
-  moreComing 

Instance Property

# moreComing

A Boolean value that indicates there are more database changes to fetch.

CloudKit JS 1.0+

``` source
readonly attribute Boolean moreComing;
```

## Discussion

`true` if there are more database changes to fetch; otherwise, `false`.

## See Also

### Response Properties

syncToken

A point in the database’s change history.

zones

The zones in the database where the changes occurred.

