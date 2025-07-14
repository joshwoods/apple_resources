

- Core Data
- Conflict resolution
- NSMergePolicy
-  Merge Policies 

API Collection

# Merge Policies

Define standard ways to handle conflicts during a save operation.

## Overview

`NSErrorMergePolicy` is the default policy. It is the only policy that requires action to correct any conflicts. The other policies make a save go through silently by making changes that follow rules specific to that policy.

## Topics

### Policies

var NSErrorMergePolicy: AnyObject

The default merge policy for all managed object contexts.

var NSMergeByPropertyStoreTrumpMergePolicy: AnyObject

A property-based merge policy that applies external changes.

var NSMergeByPropertyObjectTrumpMergePolicy: AnyObject

A property-based merge policy that applies in-memory changes.

var NSOverwriteMergePolicy: AnyObject

A merge policy that overwrites the entire stored object.

var NSRollbackMergePolicy: AnyObject

A merge policy that discards unsaved changes.

enum NSMergePolicyType

Constants that define merge policy types.

## See Also

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

