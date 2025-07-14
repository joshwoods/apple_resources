

- Core Data
- NSConstraintConflict
-  constraintValues 

Instance Property

# constraintValues

The values that the conflicting objects had when the conflict was created.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var constraintValues: [String : Any] { get }
```

## See Also

### Inspecting a Conflict

var conflictingObjects: [NSManagedObject]

The managed objects that are in conflict.

var conflictingSnapshots: [[AnyHashable : Any]]

The original property values of objects in violation of the constraint.

var constraint: [String]

The constraint that has been violated.

var databaseObject: NSManagedObject?

The object whose database row is using constraint values.

var databaseSnapshot: [String : Any]?

The values currently stored in the database.

