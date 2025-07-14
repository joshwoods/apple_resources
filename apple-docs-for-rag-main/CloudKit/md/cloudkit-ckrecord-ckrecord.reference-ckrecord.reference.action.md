

- CloudKit
- CKRecord
- CKRecord.Reference
-  CKRecord.Reference.Action 

Type Alias

# CKRecord.Reference.Action

A type that represents additional actions that occur when deleting references.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
typealias Action = CKRecord.ReferenceAction
```

## See Also

### Creating a Reference

init(recordID: CKRecord.ID, action: CKRecord.ReferenceAction)

Creates a reference object that points to the record with the specified ID.

convenience init(record: CKRecord, action: CKRecord.ReferenceAction)

Creates a reference object that points to the specified record object.

