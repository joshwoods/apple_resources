

- Foundation
-  NSOrderedSet 

Class

# NSOrderedSet

A static, ordered collection of unique objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSOrderedSet
```

## Overview

NSOrderedSet declares the programmatic interface for static sets of distinct objects. You establish a static set’s entries when it’s created, and thereafter the entries can’t be modified. NSMutableOrderedSet, on the other hand, declares a programmatic interface for dynamic sets of distinct objects. A dynamic—or mutable—set allows the addition and deletion of entries at any time, automatically allocating memory as needed.

You can use ordered sets as an alternative to arrays when the order of elements is important and performance in testing whether an object is contained in the set is a consideration—testing for membership of an array is slower than testing for membership of a set.

## Topics

### Creating an Ordered Set

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

### Initializing an Ordered Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in a given array, optionally copying the items.

convenience init(array: [Any], range: NSRange, copyItems: Bool)

Initializes a newly allocated set with the objects that are contained in the specified range of an array, optionally copying the items.

convenience init(object: Any)

Initializes a new ordered set with the object.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(orderedSet: NSOrderedSet)

Initializes a new ordered set with the contents of a set.

convenience init(orderedSet: NSOrderedSet, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the items.

convenience init(orderedSet: NSOrderedSet, range: NSRange, copyItems: Bool)

Initializes a new ordered set with the contents of an ordered set, optionally copying the items.

convenience init(set: Set&lt;AnyHashable>)

Initializes a new ordered set with the contents of a set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a new ordered set with the contents of a set, optionally copying the objects in the set.

init()

Initializes a newly allocated ordered set.

### Counting Entries

var count: Int

The number of members in the set.

### Accessing Set Members

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the ordered set.

func enumerateObjects(at: IndexSet, options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using the objects in the ordered set at the specified indexes.

func enumerateObjects((Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the ordered set.

func enumerateObjects(options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the set, using the specified enumeration options.

var firstObject: Any?

The first object in the ordered set.

var lastObject: Any?

The last object in the ordered set.

func object(at: Int) -> Any

Returns the object at the specified index of the set.

func objects(at: IndexSet) -> [Any]

Returns the objects in the ordered set at the specified indexes.

func index(of: Any) -> Int

Returns the index of the specified object.

func index(of: Any, inSortedRange: NSRange, options: NSBinarySearchingOptions, usingComparator: (Any, Any) -> ComparisonResult) -> Int

Returns the index, within a specified range, of an object compared with elements in the ordered set using a given NSComparator block.

func index(ofObjectAt: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index, from a given set of indexes, of the object in the ordered set that passes a test in a given block for a given set of enumeration options.

func index(ofObjectPassingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the object in the ordered set that passes a test in a given block.

func index(NSEnumerationOptions, ofObjectPassingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of an object in the ordered set that passes a test in a given block for a given set of enumeration options.

func indexes(ofObjectsAt: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the index, from a given set of indexes, of the object in the ordered set that passes a test in a given block for a given set of enumeration options.

func indexes(ofObjectsPassingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the index of the object in the ordered set that passes a test in a given block.

func indexes(options: NSEnumerationOptions, ofObjectsPassingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the index of an object in the ordered set that passes a test in a given block for a given set of enumeration options.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the ordered set.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the ordered set.

var reversed: NSOrderedSet

An ordered set in the reverse order.

### Key-Value Coding Support

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the receiver’s members using the specified value and key

func value(forKey: String) -> Any

Returns an ordered set containing the results of invoking `valueForKey:` using key on each of the ordered set’s objects.

### Key-Value Observing Support

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

### Comparing Sets

func isEqual(to: NSOrderedSet) -> Bool

Compares the receiving ordered set to another ordered set.

func intersects(NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given ordered set.

func intersectsSet(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving ordered set is also present in another given set.

func isSubset(of: NSOrderedSet) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given ordered set.

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving ordered set is also present in another given set.

### Creating a Sorted Array

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns an array of the ordered set’s elements sorted as specified by a given array of sort descriptors.

func sortedArray(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving ordered set’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block

func sortedArray(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving ordered set’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

### Filtering Ordered Sets

func filtered(using: NSPredicate) -> NSOrderedSet

Evaluates a given predicate against each object in the receiving ordered set and returns a new ordered set containing the objects for which the predicate returns true.

### Describing a Set

var description: String

func description(withLocale: Any?) -> String

func description(withLocale: Any?, indent: Int) -> String

### Converting Other Collections

var array: [Any]

A representation of the ordered set as an array.

var set: Set&lt;AnyHashable>

A representation of the set containing the contents of the ordered set.

### Comparing with Another Set

class NSOrderedCollectionDifference

An object representing the difference between two ordered collections.

struct NSOrderedCollectionDifferenceCalculationOptions

Constants that specify the options to use when creating an ordered collection difference.

### Initializers

init?(coder: NSCoder)

convenience init(objects: Any...)

### Default Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableOrderedSet

### Conforms To

- CVarArg
- Copyable
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

class NSMutableOrderedSet

A dynamic, ordered collection of unique objects.

