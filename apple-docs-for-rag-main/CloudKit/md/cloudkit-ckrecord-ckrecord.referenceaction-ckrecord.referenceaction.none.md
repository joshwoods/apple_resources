

- CloudKit
- CKRecord
- CKRecord.ReferenceAction
-  CKRecord.ReferenceAction.none 

Case

# CKRecord.ReferenceAction.none

A reference action that has no cascading behavior.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case none
```

## Discussion

No action occurs when you delete a record that the current record references. Deleting a parent record doesn’t delete that record’s children. The `CKReference` object still contains the ID of the deleted record and doesn’t update.

## See Also

### Deletion Reference Actions

case deleteSelf

A reference action that cascades deletions.

