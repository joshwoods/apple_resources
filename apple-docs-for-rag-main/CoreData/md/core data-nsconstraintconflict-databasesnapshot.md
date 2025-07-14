

- Core Data
- NSConstraintConflict
-  databaseSnapshot 

Instance Property

# databaseSnapshot

The values currently stored in the database.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var databaseSnapshot: [String : Any]? { get }
```

## See Also

### Inspecting a Conflict

var conflictingObjects: [NSManagedObject]

The managed objects that are in conflict.

var conflictingSnapshots: [[AnyHashable : Any]]

The original property values of objects in violation of the constraint.

var constraint: [String]

The constraint that has been violated.

var constraintValues: [String : Any]

The values that the conflicting objects had when the conflict was created.

var databaseObject: NSManagedObject?

The object whose database row is using constraint values.

