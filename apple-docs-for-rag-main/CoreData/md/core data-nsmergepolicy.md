

- Core Data
-  NSMergePolicy 

Class

# NSMergePolicy

A policy object that you use to resolve conflicts between the persistent store and in-memory versions of managed objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSMergePolicy
```

## Overview

A conflict is a mismatch between state held at two different layers in the Core Data stack. A conflict can arise when you save a managed object context and you have stale data at another layer. There are two places in which a conflict may occur:

- Between the managed object context layer and its in-memory cached state at the persistent store coordinator layer.

- Between the cached state at the persistent store coordinator and the external store (file, database, and so forth).

Conflicts are represented by instances of NSMergeConflict.

## Topics

### Getting a Merge Policy

init(merge: NSMergePolicyType)

Returns a merge policy initialized with a given policy type.

var mergeType: NSMergePolicyType

The merge type.

### Resolving a Conflict

func resolve(mergeConflicts: [Any]) throws

Resolves the conflicts in a given list.

func resolve(constraintConflicts: [NSConstraintConflict]) throws

Resolves the conflicts in a given list.

func resolve(optimisticLockingConflicts: [NSMergeConflict]) throws

Resolves the conflicts in a given list.

### Defining Merge Policies

class var error: NSMergePolicy

The default merge policy for all managed object contexts.

class var mergeByPropertyStoreTrump: NSMergePolicy

A property-based merge policy that applies external changes.

class var mergeByPropertyObjectTrump: NSMergePolicy

A property-based merge policy that applies in-memory changes.

class var overwrite: NSMergePolicy

A merge policy that overwrites the entire stored object.

class var rollback: NSMergePolicy

A merge policy that discards unsaved changes.

Merge Policies

Define standard ways to handle conflicts during a save operation.

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

class NSMergeConflict

An encapsulation of conflicts that occur during an attempt to save changes in a managed object context.

class NSQueryGenerationToken

A token that indicates which generation of the persistent store is being accessed.

