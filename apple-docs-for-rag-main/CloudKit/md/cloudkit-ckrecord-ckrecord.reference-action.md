

- CloudKit
- CKRecord
- CKRecord.Reference
-  action 

Instance Property

# action

The ownership behavior for the records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var action: CKRecord.ReferenceAction { get }
```

## Discussion

The value in this property determines which action, if any, to take when deleting the target of the reference object — that is, the object that the recordID property points to. When this property is CKRecord.ReferenceAction.deleteSelf, deleting the target object deletes any records that contain that reference in one of their fields. When this property is CKRecord.ReferenceAction.none, deleting the target object doesn’t delete any additional objects.

## See Also

### Getting the Reference Attributes

var recordID: CKRecord.ID

The ID of the referenced record.

enum ReferenceAction

Constants that indicate the behavior when deleting a referenced record.

