

- CKTool JS
- CKDBLookupRecordsResponse
-  recordResults 

Instance Property

# recordResults

The array of `CKDBRecordResult` objects that represent a record.

CKTool JS 1.2.15+

``` source
attribute CKDBRecordResult[] recordResults;
```

## Discussion

`CKDBRecordResult` objects are used for representing a record when the lookup operation can potentially return deleted records or fail partially when looking up some of the record.

