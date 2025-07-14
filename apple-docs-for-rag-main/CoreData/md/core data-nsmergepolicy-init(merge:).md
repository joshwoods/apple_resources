

- Core Data
- NSMergePolicy
-  init(merge:) 

Initializer

# init(merge:)

Returns a merge policy initialized with a given policy type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(merge ty: NSMergePolicyType)
```

## Parameters 

`ty`  

A merge policy type.

## Return Value

A merge policy initialized with a given policy type.

## Discussion

If you override this method in a subclass, you should invoke the superclass’s implementation with the merge policy that is closest to the behavior you want.

- This will make it easier to use the superclass’s implementation of resolve(mergeConflicts:) and then customize the results.

- Due to the complexity of merging to-many relationships, this class is designed with the expectation that you call super as the base implementation.

## See Also

### Related Documentation

Core Data Model Versioning and Data Migration Programming Guide

### Getting a Merge Policy

var mergeType: NSMergePolicyType

The merge type.

