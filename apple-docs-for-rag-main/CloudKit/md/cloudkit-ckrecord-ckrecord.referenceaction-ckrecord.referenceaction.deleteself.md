

- CloudKit
- CKRecord
- CKRecord.ReferenceAction
-  CKRecord.ReferenceAction.deleteSelf 

Case

# CKRecord.ReferenceAction.deleteSelf

A reference action that cascades deletions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case deleteSelf
```

## Discussion

CloudKit deletes any records that contain `CKReference` objects pointing to the current record. The deletion of the additional records can trigger further deletions as the action cascades. The deletions are asynchronous in the default zone and immediate in a custom zone.

## See Also

### Deletion Reference Actions

case none

A reference action that has no cascading behavior.

