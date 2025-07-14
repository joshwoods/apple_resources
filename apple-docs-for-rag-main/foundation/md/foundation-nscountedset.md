

- Foundation
-  NSCountedSet 

Class

# NSCountedSet

A mutable, unordered collection of distinct objects that may appear more than once in the collection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSCountedSet
```

## Overview

Each distinct object inserted into an NSCountedSet object has a counter associated with it. NSCountedSet keeps track of the number of times objects are inserted and requires that objects be removed the same number of times. Thus, there is only one instance of an object in an NSSet object even if the object has been added to the set multiple times. The count method defined by the superclass NSSet has special significance; it returns the number of distinct objects, not the total number of times objects are represented in the set. The NSSet and NSMutableSet classes are provided for static and dynamic sets, respectively, whose elements are distinct.

While NSCountedSet and doc://com.apple.documentation/documentation/corefoundation/cfbag-s1l are not toll-free bridged, they provide similar functionality. For more information about `CFBag`, see the doc://com.apple.documentation/documentation/corefoundation/cfbag-s1l.

### Subclassing Notes

Because NSCountedSet is not a class cluster, it does not have primitive methods that provide the basis for its implementation. In general, there should be little need for subclassing.

#### Methods to Override

If you subclass NSCountedSet, you must override any method of which you want to change the behavior.

If you change the primitive behavior of an NSCountedSet, for instance if you change how objects are stored, you must override all of the affected methods. These include:

- add(_:)

- remove(_:)

- objectEnumerator()

- count(for:)

If you change the primitive behavior, you must also override the primitive methods of NSSet and NSMutableSet.

## Topics

### Initializing a Counted Set

convenience init(array: [Any])

Returns a counted set object initialized with the contents of a given array.

convenience init(set: Set&lt;AnyHashable>)

Returns a counted set object initialized with the contents of a given set.

init(capacity: Int)

Returns a counted set object initialized with enough memory to hold a given number of objects.

### Adding and Removing Entries

func add(Any)

Adds a given object to the set.

func remove(Any)

Removes a given object from the set.

### Examining a Counted Set

func count(for: Any) -> Int

Returns the count associated with a given object in the set.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the set once, independent of its count.

## Relationships

### Inherits From

- NSMutableSet

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

## See Also

### Specialized Sets

class NSOrderedSet

A static, ordered collection of unique objects.

class NSMutableOrderedSet

A dynamic, ordered collection of unique objects.

