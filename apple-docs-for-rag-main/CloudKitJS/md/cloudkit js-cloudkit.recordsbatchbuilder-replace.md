

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  replace 

Instance Method

# replace

Replaces one or more records with the specified records.

CloudKit JS 1.0+

``` source
CloudKit.RecordsBatchBuilder replace(
    CloudKit.Record|CloudKit.Record[] records,
 optional Object options
);
```

## Parameters 

`records`  

A CloudKit.Record dictionary representing the replacement record, if you are replacing a single record. If you are replacing multiple records, this parameter is an array of replacement CloudKit.Record dictionaries. The CloudKit.Record dictionaries must contain the `recordChangeTag` key. Only the values of the fields in these dictionaries are replaced. The other field values are set to `null`.

`options`  

A dictionary containing options for this operation. This parameter contains a single `desiredKeys` key that is an array of field names (`String` values). Only the fields specified in the array are set.

## Return Value

The object that received this method call.

## Discussion

The fields whose values you do not specify are set to `null`.

## See Also

### Replacing Records

forceReplace

Replaces one or more records with the specified records regardless of conflicts.

