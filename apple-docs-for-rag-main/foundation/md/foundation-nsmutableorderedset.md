

- Foundation
-  NSMutableOrderedSet 

Class

# NSMutableOrderedSet

A dynamic, ordered collection of unique objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableOrderedSet
```

## Overview

NSMutableOrderedSet objects are not like C arrays. That is, even though you may specify a size when you create a mutable ordered set, the specified size is regarded as a “hint”; the actual size of the set is still 0. This means that you cannot insert an object at an index greater than the current count of an set. For example, if a set contains two objects, its size is 2, so you can add objects at indices 0, 1, or 2. Index 3 is illegal and out of bounds; if you try to add an object at index 3 (when the size of the array is 2), `NSMutableOrderedSet` raises an exception.

## Topics

### Creating a Mutable Ordered Set

init(capacity: Int)

Returns an initialized mutable ordered set with a given initial capacity.

init()

Initializes a newly allocated mutable ordered set.

### Adding, Removing, and Reordering Entries

func add(Any)

Appends a given object to the end of the mutable ordered set, if it is not already a member.

func add(UnsafePointer&lt;AnyObject>?, count: Int)

Appends the given number of objects from a given C array to the end of the mutable ordered set.

func addObjects(from: [Any])

Appends to the end of the mutable ordered set each object contained in a given array that is not already a member.

func insert(Any, at: Int)

Inserts the given object at the specified index of the mutable ordered set, if it is not already a member.

func insert([Any], at: IndexSet)

Inserts the objects in the array at the specified indexes.

func remove(Any)

Removes a given object from the mutable ordered set.

func removeObject(at: Int)

Removes a the object at the specified index from the mutable ordered set.

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the mutable ordered set.

func removeObjects(in: [Any])

Removes the objects in the array from the mutable ordered set.

func removeObjects(in: NSRange)

Removes from the mutable ordered set each of the objects within a given range.

func removeAllObjects()

Removes all the objects from the mutable ordered set.

func replaceObject(at: Int, with: Any)

Replaces the object at the specified index with the new object.

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects at the specified indexes with the new objects.

func replaceObjects(in: NSRange, with: UnsafePointer&lt;AnyObject>?, count: Int)

Replaces the objects in the receiving mutable ordered set at the range with the specified number of objects from a given C array.

func setObject(Any, at: Int)

Appends or replaces the object at the specified index.

func moveObjects(at: IndexSet, to: Int)

Moves the objects at the specified indexes to the new location.

func exchangeObject(at: Int, withObjectAt: Int)

Exchanges the object at the specified index with the object at the other index.

func filter(using: NSPredicate)

Evaluates a given predicate against the mutable ordered set’s content and leaves only objects that match.

### Sorting Entries

func sort(using: [NSSortDescriptor])

Sorts the receiving ordered set using a given array of sort descriptors.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the comparison method specified by the comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

func sortRange(NSRange, options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the specified range of the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

### Combining and Recombining Entries

func intersect(NSOrderedSet)

Removes from the receiving ordered set each object that isn’t a member of another ordered set.

func intersectSet(Set&lt;AnyHashable>)

Removes from the receiving ordered set each object that isn’t a member of another set.

func minus(NSOrderedSet)

Removes each object in another given ordered set from the receiving mutable ordered set, if present.

func minusSet(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving mutable ordered set, if present.

func union(NSOrderedSet)

Adds each object in another given ordered set to the receiving mutable ordered set, if not present.

func unionSet(Set&lt;AnyHashable>)

Adds each object in another given set to the receiving mutable ordered set, if not present.

### Initializers

init?(coder: NSCoder)

### Subscripts

subscript(Int) -> Any

Returns the object at the specified index of the set.

## Relationships

### Inherits From

- NSOrderedSet

### Conforms To

- CVarArg
- CustomDebugStringConvertible
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

class NSCountedSet

A mutable, unordered collection of distinct objects that may appear more than once in the collection.

class NSOrderedSet

A static, ordered collection of unique objects.

