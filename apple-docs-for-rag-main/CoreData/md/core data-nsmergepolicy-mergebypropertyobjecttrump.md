

- Core Data
- NSMergePolicy
-  mergeByPropertyObjectTrump 

Type Property

# mergeByPropertyObjectTrump

A property-based merge policy that applies in-memory changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class var mergeByPropertyObjectTrump: NSMergePolicy { get }
```

## Discussion

A policy that merges conflicts between the persistent store’s version of the object and the current in-memory version by individual property, with in-memory changes trumping external changes.

## See Also

### Defining Merge Policies

class var error: NSMergePolicy

The default merge policy for all managed object contexts.

class var mergeByPropertyStoreTrump: NSMergePolicy

A property-based merge policy that applies external changes.

class var overwrite: NSMergePolicy

A merge policy that overwrites the entire stored object.

class var rollback: NSMergePolicy

A merge policy that discards unsaved changes.

Merge Policies

Define standard ways to handle conflicts during a save operation.

