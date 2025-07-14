

- CKTool JS
- CKDBRecord
-  fields 

Instance Property

# fields

The dictionary of key-value pairs whose keys are the record field names and values are field-value dictionaries.

CKTool JS 1.2.15+

``` source
attribute dictionary fields;
```

## Discussion

Values in this dictionary conform to `CKDBRecordFieldValue`. `CKDBRecordFieldValue` is the root of the hierarchy of valid record field value types, such as `CKDBRecordFieldStringValue`.

