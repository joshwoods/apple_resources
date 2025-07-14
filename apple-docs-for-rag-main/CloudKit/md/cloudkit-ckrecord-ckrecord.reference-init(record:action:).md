

- CloudKit
- CKRecord
- CKRecord.Reference
-  init(record:action:) 

Initializer

# init(record:action:)

Creates a reference object that points to the specified record object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init(
    record: CKRecord,
    action: CKRecord.ReferenceAction
)
```

## Parameters 

`record`  

The target record of the reference.

`action`  

The ownership options to use for the records. If you specify the CKRecord.ReferenceAction.deleteSelf option, the object that the `recordID` parameter references becomes the owner of (or acts as the parent of) any objects that use this reference object. For a list of possible values, see CKRecord.ReferenceAction.

## Return Value

An initialized reference object that points to the specified record, or `nil` if CloudKit can’t initialize the reference.

## Discussion

Use this method to initialize a reference to a local record object. The local record can be one that you create or one that you fetch from the server.

When you create a reference object for use in a search predicate, the predicate ignores the value in the `action` parameter. Search predicates use only the ID of the record during their comparison.

## See Also

### Creating a Reference

init(recordID: CKRecord.ID, action: CKRecord.ReferenceAction)

Creates a reference object that points to the record with the specified ID.

typealias Action

A type that represents additional actions that occur when deleting references.

