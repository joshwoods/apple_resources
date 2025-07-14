

- CKTool JS
- CKDBModifyRecordRequestBody
-  fields 

Instance Property

# fields

The dictionary of key-value pairs whose keys are the record field names and values are field-value dictionaries.

CKTool JS 1.2.15+

``` source
attribute dictionary fields;
```

## Discussion

The values in this fields dictionary can be any kind of `CKDBRecordFieldValue` object. For example, `CKDBRecordFieldInt64Value`.

