

- Core Data
-  NSOverwriteMergePolicy 

Global Variable

# NSOverwriteMergePolicy

A merge policy that overwrites the entire stored object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var NSOverwriteMergePolicy: AnyObject
```

## Discussion

This policy merges conflicts between the persistent store’s version of the object and the current in-memory version by saving the entire in-memory object to the persistent store.

## See Also

### Policies

var NSErrorMergePolicy: AnyObject

The default merge policy for all managed object contexts.

var NSMergeByPropertyStoreTrumpMergePolicy: AnyObject

A property-based merge policy that applies external changes.

var NSMergeByPropertyObjectTrumpMergePolicy: AnyObject

A property-based merge policy that applies in-memory changes.

var NSRollbackMergePolicy: AnyObject

A merge policy that discards unsaved changes.

enum NSMergePolicyType

Constants that define merge policy types.

