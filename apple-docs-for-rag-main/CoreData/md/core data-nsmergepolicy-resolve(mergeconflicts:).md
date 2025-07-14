

- Core Data
- NSMergePolicy
-  resolve(mergeConflicts:) 

Instance Method

# resolve(mergeConflicts:)

Resolves the conflicts in a given list.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func resolve(mergeConflicts list: [Any]) throws
```

## Parameters 

`list`  

An array of merge conflicts (instances of NSMergeConflict).

## Discussion

If you override this method in a subclass, you should typically invoke the superclass’s implementation in addition to performing your own operations.

## See Also

### Resolving a Conflict

func resolve(constraintConflicts: [NSConstraintConflict]) throws

Resolves the conflicts in a given list.

func resolve(optimisticLockingConflicts: [NSMergeConflict]) throws

Resolves the conflicts in a given list.

