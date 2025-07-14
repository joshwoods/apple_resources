

- Foundation
-  NSFastEnumeration 

Protocol

# NSFastEnumeration

A protocol that objects adopt to support fast enumeration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSFastEnumeration
```

## Overview

The abstract class NSEnumerator provides a convenience implementation that uses nextObject() to return items one at a time.

## Topics

### Enumeration

func countByEnumerating(with: UnsafeMutablePointer&lt;NSFastEnumerationState>, objects: AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, count: Int) -> Int

Returns by reference a C array of objects over which the sender should iterate, and as the return value the number of objects in the array.

**Required**

### Constants

struct NSFastEnumerationState

This defines the structure used as contextual information in the NSFastEnumeration protocol.

## Relationships

### Conforming Types

- FileManager.DirectoryEnumerator
- NSArray
- NSCountedSet
- NSDictionary
- NSEnumerator
- NSHashTable
- NSMapTable
- NSMutableArray
- NSMutableDictionary
- NSMutableOrderedSet
- NSMutableSet
- NSOrderedCollectionDifference
- NSOrderedSet
- NSPointerArray
- NSSet

## See Also

### Iteration

class NSEnumerator

An abstract class whose subclasses enumerate collections of objects, such as arrays and dictionaries.

struct NSFastEnumerationIterator

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

struct NSEnumerationOptions

Options for block enumeration operations.

struct NSSortOptions

Options for block sorting operations.

