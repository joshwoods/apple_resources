

- Core Data
-  NSErrorMergePolicy 

Global Variable

# NSErrorMergePolicy

The default merge policy for all managed object contexts.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var NSErrorMergePolicy: AnyObject
```

## Discussion

If a save fails because of conflicting objects, you can find the IDs of those objects in error’s `userInfo` dictionary. Use the NSInsertedObjectsKey and NSUpdatedObjectsKey keys to extract the object IDs.

## See Also

### Policies

var NSMergeByPropertyStoreTrumpMergePolicy: AnyObject

A property-based merge policy that applies external changes.

var NSMergeByPropertyObjectTrumpMergePolicy: AnyObject

A property-based merge policy that applies in-memory changes.

var NSOverwriteMergePolicy: AnyObject

A merge policy that overwrites the entire stored object.

var NSRollbackMergePolicy: AnyObject

A merge policy that discards unsaved changes.

enum NSMergePolicyType

Constants that define merge policy types.

