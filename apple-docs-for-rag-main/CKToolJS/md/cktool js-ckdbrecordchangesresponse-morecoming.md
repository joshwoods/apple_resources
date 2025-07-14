

- CKTool JS
- CKDBRecordChangesResponse
-  moreComing 

Instance Property

# moreComing

A Boolean value that indicates whether there are more changes to request.

CKTool JS 1.2.15+

``` source
attribute boolean moreComing;
```

## Discussion

If `moreComing` is `true`, request more changes using the value of the included `changeToken`. If `moreComing` is `false`, there are no more changes.

