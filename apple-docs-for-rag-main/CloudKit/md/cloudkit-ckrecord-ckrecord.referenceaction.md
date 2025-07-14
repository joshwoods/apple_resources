

- CloudKit
- CKRecord
-  CKRecord.ReferenceAction 

Enumeration

# CKRecord.ReferenceAction

Constants that indicate the behavior when deleting a referenced record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
enum ReferenceAction
```

## Topics

### Deletion Reference Actions

case none

A reference action that has no cascading behavior.

case deleteSelf

A reference action that cascades deletions.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Reference Attributes

var action: CKRecord.ReferenceAction

The ownership behavior for the records.

var recordID: CKRecord.ID

The ID of the referenced record.

