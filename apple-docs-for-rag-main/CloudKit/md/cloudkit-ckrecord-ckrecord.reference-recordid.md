

- CloudKit
- CKRecord
- CKRecord.Reference
-  recordID 

Instance Property

# recordID

The ID of the referenced record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var recordID: CKRecord.ID { get }
```

## Discussion

Use the ID in this property to fetch the record on the other end of the link.

## See Also

### Getting the Reference Attributes

var action: CKRecord.ReferenceAction

The ownership behavior for the records.

enum ReferenceAction

Constants that indicate the behavior when deleting a referenced record.

