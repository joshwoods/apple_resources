

- Core Data
- NSConstraintConflict
-  init(constraint:database:databaseSnapshot:conflicting:conflictingSnapshots:) 

Initializer

# init(constraint:database:databaseSnapshot:conflicting:conflictingSnapshots:)

Initializes a constraint conflict.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    constraint contraint: [String],
    database databaseObject: NSManagedObject?,
    databaseSnapshot: [AnyHashable : Any]?,
    conflicting conflictingObjects: [NSManagedObject],
    conflictingSnapshots: [Any]
)
```

