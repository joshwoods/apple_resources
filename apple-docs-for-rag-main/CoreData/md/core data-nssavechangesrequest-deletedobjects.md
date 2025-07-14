

- Core Data
- NSSaveChangesRequest
-  deletedObjects 

Instance Property

# deletedObjects

The objects that were deleted in the calling context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var deletedObjects: Set? { get }
```

## See Also

### Getting Information about a Request

var insertedObjects: Set&lt;NSManagedObject>?

The objects that were inserted into the calling context.

var updatedObjects: Set&lt;NSManagedObject>?

The objects that were modified in the calling context.

var lockedObjects: Set&lt;NSManagedObject>?

The objects that were flagged for optimistic locking on the calling context.

