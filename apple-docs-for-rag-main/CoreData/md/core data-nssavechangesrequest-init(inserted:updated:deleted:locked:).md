

- Core Data
- NSSaveChangesRequest
-  init(inserted:updated:deleted:locked:) 

Initializer

# init(inserted:updated:deleted:locked:)

Initializes a save changes request with collections of given changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    inserted insertedObjects: Set?,
    updated updatedObjects: Set?,
    deleted deletedObjects: Set?,
    locked lockedObjects: Set?
)
```

## Parameters 

`insertedObjects`  

Objects that were inserted into the calling context.

`updatedObjects`  

Objects that were updated in the calling context.

`deletedObjects`  

Objects that were deleted in the calling context.

`lockedObjects`  

Objects that were flagged for optimistic locking on the calling context.

## Return Value

A save changes request initialized with the given changes.

