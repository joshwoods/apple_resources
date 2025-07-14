

- Core Data
- NSMergePolicy
-  error 

Type Property

# error

The default merge policy for all managed object contexts.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class var error: NSMergePolicy { get }
```

## Discussion

If a save fails because of conflicting objects, you can find the IDs of those objects in error’s `userInfo` dictionary. Use the NSInsertedObjectsKey and NSUpdatedObjectsKey keys to extract the object IDs.

## See Also

### Defining Merge Policies

class var mergeByPropertyStoreTrump: NSMergePolicy

A property-based merge policy that applies external changes.

class var mergeByPropertyObjectTrump: NSMergePolicy

A property-based merge policy that applies in-memory changes.

class var overwrite: NSMergePolicy

A merge policy that overwrites the entire stored object.

class var rollback: NSMergePolicy

A merge policy that discards unsaved changes.

Merge Policies

Define standard ways to handle conflicts during a save operation.

