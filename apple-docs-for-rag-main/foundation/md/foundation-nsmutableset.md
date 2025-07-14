

- Foundation
-  NSMutableSet 

Class

# NSMutableSet

A dynamic unordered collection of unique objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableSet
```

## Overview

You can use this type in Swift instead of a Set in cases that require reference semantics.

The `NSMutableSet` class declares the programmatic interface to a mutable, unordered collection of distinct objects.

The NSCountedSet class, which is a concrete subclass of `NSMutableSet`, supports mutable sets that can contain multiple instances of the same element. The NSSet class supports creating and managing immutable sets.

NSMutableSet is “toll-free bridged” with its Core Foundation counterpart, CFMutableSet. See Toll-Free Bridging for more information.

### Subclassing Notes

There should be little need of subclassing. If you need to customize behavior, it is often better to consider composition instead of subclassing.

#### Methods to Override

In a subclass, you must override both of its primitive methods:

- add(_:)

- remove(_:)

You must also override the primitive methods of the NSSet class.

## Topics

### Creating a mutable set

init(capacity: Int)

Returns an initialized mutable set with a given initial capacity.

init()

Initializes a newly allocated set.

### Adding and removing entries

func add(Any)

Adds a given object to the set, if it is not already a member.

func filter(using: NSPredicate)

Evaluates a given predicate against the set’s content and removes from the set those objects for which the predicate returns false.

func remove(Any)

Removes a given object from the set.

func removeAllObjects()

Empties the set of all of its members.

func addObjects(from: [Any])

Adds to the set each object contained in a given array that is not already a member.

### Combining and recombining sets

func union(Set&lt;AnyHashable>)

Adds each object in another given set to the receiving set, if not present.

func minus(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving set, if present.

func intersect(Set&lt;AnyHashable>)

Removes from the receiving set each object that isn’t a member of another given set.

func setSet(Set&lt;AnyHashable>)

Empties the receiving set, then adds each object contained in another given set.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSSet

### Inherited By

- NSCountedSet

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

