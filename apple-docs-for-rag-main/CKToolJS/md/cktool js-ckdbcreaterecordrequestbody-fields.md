

- CKTool JS
- CKDBCreateRecordRequestBody
-  fields 

Instance Property

# fields

The dictionary of key-value pairs whose keys are the record field names and values are field-value dictionaries.

CKTool JS 1.2.15+

``` source
attribute dictionary fields;
```

## Discussion

Missing fields in this dictionary are set to `null`. See `CKDBRecordFieldValue`.

