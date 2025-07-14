

- Foundation
-  NSEnumerator 

Class

# NSEnumerator

An abstract class whose subclasses enumerate collections of objects, such as arrays and dictionaries.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSEnumerator
```

## Overview

All creation methods are defined in the collection classes—such as NSArray, NSSet, and NSDictionary—which provide special NSEnumerator objects with which to enumerate their contents. For example, `NSArray` has two methods that return an NSEnumerator object: objectEnumerator() and reverseObjectEnumerator(). `NSDictionary` also has two methods that return an NSEnumerator object: keyEnumerator() and objectEnumerator(). These methods let you enumerate the contents of a dictionary by key or by value, respectively.

You send nextObject() repeatedly to a newly created NSEnumerator object to have it return the next object in the original collection. When the collection is exhausted, `nil` is returned. You cannot “reset” an enumerator after it has exhausted its collection. To enumerate a collection again, you need a new enumerator.

The enumerator subclasses used by `NSArray`, `NSDictionary`, and `NSSet` retain the collection during enumeration. When the enumeration is exhausted, the collection is released.

Note

In Objective-C, it is not safe to modify a mutable collection while enumerating through it. Some enumerators may currently allow enumeration of a collection that is modified, but this behavior is not guaranteed to be supported in the future.

## Topics

### Getting the Enumerated Objects

var allObjects: [Any]

The array of unenumerated objects.

func nextObject() -> Any?

Returns the next object from the collection being enumerated.

### Default Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- FileManager.DirectoryEnumerator

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFastEnumeration
- NSObjectProtocol
- Sequence

## See Also

### Iteration

protocol NSFastEnumeration

A protocol that objects adopt to support fast enumeration.

struct NSFastEnumerationIterator

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

struct NSEnumerationOptions

Options for block enumeration operations.

struct NSSortOptions

Options for block sorting operations.

