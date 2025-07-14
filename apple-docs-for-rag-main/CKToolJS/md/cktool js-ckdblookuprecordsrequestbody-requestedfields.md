

- CKTool JS
- CKDBLookupRecordsRequestBody
-  requestedFields 

Instance Property

# requestedFields

The array of record field names that limits the amount of data returned in this operation.

CKTool JS 1.2.15+

``` source
attribute string[]? requestedFields;
```

## Discussion

The server only returns the fields specified in the array. If omitted, the server returns all record fields. If set to an empty array, the server returns record metadata without the fields.

