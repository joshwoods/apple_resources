

- Core Data
-  NSConstraintConflict 

Class

# NSConstraintConflict

An encapsulation of conflicts that occur during an attempt to save a managed object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSConstraintConflict
```

## Overview

A constraint conflict occurs when your data model is using unique constraints and one or more managed objects are violating that constraint.

When this error occurs, the error instance can be interrogated to determine which instance of NSManagedObject is violating the constraint and which property on the NSManagedObject instance is in violation.

## Topics

### Initializing a Conflict

init(constraint: [String], database: NSManagedObject?, databaseSnapshot: [AnyHashable : Any]?, conflicting: [NSManagedObject], conflictingSnapshots: [Any])

Initializes a constraint conflict.

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

var databaseSnapshot: [String : Any]?

The values currently stored in the database.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Conflict Management

class NSMergeConflict

An encapsulation of conflicts that occur during an attempt to save changes in a managed object context.

class NSMergePolicy

A policy object that you use to resolve conflicts between the persistent store and in-memory versions of managed objects.

class NSQueryGenerationToken

A token that indicates which generation of the persistent store is being accessed.

