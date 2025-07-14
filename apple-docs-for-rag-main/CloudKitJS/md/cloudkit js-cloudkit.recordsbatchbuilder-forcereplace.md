

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  forceReplace 

Instance Method

# forceReplace

Replaces one or more records with the specified records regardless of conflicts.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder forceReplace(
    CloudKit.Record|CloudKit.Record[] records,
 optional Object options
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the replacement record, if you are replacing a single record. If you are replacing multiple records, this value is an array of replacement CloudKit.Record dictionaries. The `recordChangeTag` key is not required in the CloudKit.Record dictionaries. Only the values of the fields in these dictionaries are replaced. The other field values are set to `null`.

`options`  

A dictionary containing options for this operation. This parameter contains a single `desiredKeys` key that is an array of field names (`String` values). Only the fields specified in the array are set.

## Return Value

The object that received this method call.

## Discussion

Creates records if they don’t exist.

## See Also

### Replacing Records

replace

Replaces one or more records with the specified records.

