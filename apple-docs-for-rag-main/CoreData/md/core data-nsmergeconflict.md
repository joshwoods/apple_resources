

- Core Data
-  NSMergeConflict 

Class

# NSMergeConflict

An encapsulation of conflicts that occur during an attempt to save changes in a managed object context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSMergeConflict
```

## Overview

A conflict can occur in two situations:

- Between the managed object context and its in-memory cached state at the persistent store coordinator layer.

- Between the cached state at the persistent store coordinator layer and the external store (file, database, and so forth). In this case, the merge conflict has a cached snapshot and a persisted snapshot. The source object is also provided as a convenience, but it is not directly involved in the conflict.

Snapshot dictionaries include values for all attributes and to-one relationships, but not to-many relationships. Relationship values are `NSManagedObjectID` references. To-many relationships must be pulled from the persistent store as needed.

## Topics

### Initializing a Merge Conflict

init(source: NSManagedObject, newVersion: Int, oldVersion: Int, cachedSnapshot: [String : Any]?, persistedSnapshot: [String : Any]?)

Initializes a merge conflict.

### Accessing Merge Conflict Details

var sourceObject: NSManagedObject

The source object for the conflict.

var objectSnapshot: [String : Any]?

A dictionary containing the values of the source object.

var cachedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store coordinator layer.

var persistedSnapshot: [String : Any]?

A dictionary containing the values of the source object held in the persistent store.

var newVersionNumber: Int

The new version number for the change.

var oldVersionNumber: Int

The old version number for the change.

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

class NSConstraintConflict

An encapsulation of conflicts that occur during an attempt to save a managed object.

class NSMergePolicy

A policy object that you use to resolve conflicts between the persistent store and in-memory versions of managed objects.

class NSQueryGenerationToken

A token that indicates which generation of the persistent store is being accessed.

