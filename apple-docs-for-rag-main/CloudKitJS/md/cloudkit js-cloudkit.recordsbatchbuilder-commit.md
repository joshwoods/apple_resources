

- CloudKit JS
- CloudKit.RecordsBatchBuilder
-  commit 

Instance Method

# commit

Executes the operations on the database that created this batch builder object.

CloudKit JS 1.0+

``` source
Promise commit();
```

## Return Value

A `Promise` object that resolves to a RecordsResponse object if the operation succeeds; otherwise, a CKError object.

