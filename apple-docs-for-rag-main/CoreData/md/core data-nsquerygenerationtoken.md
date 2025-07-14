

- Core Data
-  NSQueryGenerationToken 

Class

# NSQueryGenerationToken

A token that indicates which generation of the persistent store is being accessed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class NSQueryGenerationToken
```

## Mentioned in 

Accessing data when the store changes

## Overview

When a managed object context is pinned to a specific generation of the app data, a query generation token will be associated with that context.

## Topics

### Identifying Generations of App Data

class var current: NSQueryGenerationToken

A token that informs a context to use the current generation.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Conflict Management

class NSConstraintConflict

An encapsulation of conflicts that occur during an attempt to save a managed object.

class NSMergeConflict

An encapsulation of conflicts that occur during an attempt to save changes in a managed object context.

class NSMergePolicy

A policy object that you use to resolve conflicts between the persistent store and in-memory versions of managed objects.

