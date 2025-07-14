

- Core Data
- NSSaveChangesRequest
-  lockedObjects 

Instance Property

# lockedObjects

The objects that were flagged for optimistic locking on the calling context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var lockedObjects: Set? { get }
```

## Discussion

Objects are flagged for optimistic locking with detectConflicts(for:).

## See Also

### Getting Information about a Request

var insertedObjects: Set&lt;NSManagedObject>?

The objects that were inserted into the calling context.

var updatedObjects: Set&lt;NSManagedObject>?

The objects that were modified in the calling context.

var deletedObjects: Set&lt;NSManagedObject>?

The objects that were deleted in the calling context.

