

- Core Data
- NSMergePolicy
-  rollback 

Type Property

# rollback

A merge policy that discards unsaved changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class var rollback: NSMergePolicy { get }
```

## Discussion

This policy merges conflicts between the persistent store’s version of the object and the current in-memory version by discarding unsaved changes.

## See Also

### Defining Merge Policies

class var error: NSMergePolicy

The default merge policy for all managed object contexts.

class var mergeByPropertyStoreTrump: NSMergePolicy

A property-based merge policy that applies external changes.

class var mergeByPropertyObjectTrump: NSMergePolicy

A property-based merge policy that applies in-memory changes.

class var overwrite: NSMergePolicy

A merge policy that overwrites the entire stored object.

Merge Policies

Define standard ways to handle conflicts during a save operation.

