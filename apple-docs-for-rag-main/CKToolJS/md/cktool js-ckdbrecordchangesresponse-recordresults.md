

- CKTool JS
- CKDBRecordChangesResponse
-  recordResults 

Instance Property

# recordResults

An array of record result objects that provide details about the records.

CKTool JS 1.2.15+

``` source
attribute CKDBRecordResult[] recordResults;
```

## Discussion

CKDBRecordResult objects are used for representing a record when the lookup operation can potentially return deleted records or fail partially when looking up some of the record.

