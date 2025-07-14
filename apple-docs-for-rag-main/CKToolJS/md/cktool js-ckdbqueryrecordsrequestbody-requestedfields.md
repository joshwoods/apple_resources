

- CKTool JS
- CKDBQueryRecordsRequestBody
-  requestedFields 

Instance Property

# requestedFields

An array of record field names that limit the amount of data the server returns in this operation.

CKTool JS 1.2.15+

``` source
attribute string[]? requestedFields;
```

## Discussion

The server only returns the fields specified in the array. If omitted, the server returns all record fields. If set to an empty array, the server returns record metadata without the fields.

