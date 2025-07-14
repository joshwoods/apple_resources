

- Core Data
-  NSMergeByPropertyStoreTrumpMergePolicy 

Global Variable

# NSMergeByPropertyStoreTrumpMergePolicy

A property-based merge policy that applies external changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var NSMergeByPropertyStoreTrumpMergePolicy: AnyObject
```

## Discussion

A policy that merges conflicts between the persistent store’s version of the object and the current in-memory version by individual property, with external changes trumping in-memory changes.

## See Also

### Policies

var NSErrorMergePolicy: AnyObject

The default merge policy for all managed object contexts.

var NSMergeByPropertyObjectTrumpMergePolicy: AnyObject

A property-based merge policy that applies in-memory changes.

var NSOverwriteMergePolicy: AnyObject

A merge policy that overwrites the entire stored object.

var NSRollbackMergePolicy: AnyObject

A merge policy that discards unsaved changes.

enum NSMergePolicyType

Constants that define merge policy types.

