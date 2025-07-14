

- CKTool JS
- CKDBModifyRecordRequestBody
-  recordChangeTag 

Instance Property

# recordChangeTag

A string containing the server change token for the record.

CKTool JS 1.2.15+

``` source
attribute string? recordChangeTag;
```

## Discussion

Use this tag to indicate which version of the record you last fetched. This tag is required unless force parameter for updateRecord operation is set to true.

