

- Foundation
-  NSMutableArray 

Class

# NSMutableArray

A dynamic ordered collection of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableArray
```

## Overview

You can use this type in Swift instead of an Array variable in cases that require reference semantics.

The `NSMutableArray` class declares the programmatic interface to objects that manage a modifiable array of objects. This class adds insertion and deletion operations to the basic array-handling behavior inherited from NSArray.

NSMutableArray is “toll-free bridged” with its Core Foundation counterpart, CFMutableArray. See Toll-Free Bridging for more information.

### Accessing Values Using Subscripting

In addition to the provided instance methods, such as replaceObject(at:with:), you can access `NSArray` values by their indexes using *subscripting*.

- Swift
- Objective-C

```
mutableArray[3] = "someValue"
```

```
mutableArray[3] = @"someValue";
```

### Subclassing Notes

There is typically little reason to subclass `NSMutableArray`. The class does well what it is designed to do—maintain a mutable, ordered collection of objects. But there are situations where a custom `NSArray` object might come in handy. Here are a few possibilities:

- Changing how `NSMutableArray` stores the elements of its collection. You might do this for performance reasons or for better compatibility with legacy code.

- Acquiring more information about what is happening to the collection (for example, statistics gathering).

#### Methods to Override

`NSMutableArray` defines five primitive methods:

- insert(_:at:)

- removeObject(at:)

- add(_:)

- removeLastObject()

- replaceObject(at:with:)

In a subclass, you must override all these methods. You must also override the primitive methods of the NSArray class.

## Topics

### Creating and Initializing a Mutable Array

init?(contentsOfURL: URL)

Creates and returns a mutable array containing the contents specified by a given URL.

init()

Initializes a newly allocated array.

init(capacity: Int)

Returns an array, initialized with enough memory to initially hold a given number of objects.

### Adding Objects

func add(Any)

Inserts a given object at the end of the array.

func addObjects(from: [Any])

Adds the objects contained in another given array to the end of the receiving array’s content.

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

func insert([Any], at: IndexSet)

Inserts the objects in the provided array into the receiving array at the specified indexes.

### Removing Objects

func removeAllObjects()

Empties the array of all its elements.

func removeLastObject()

Removes the object with the highest-valued index in the array

func remove(Any)

Removes all occurrences in the array of a given object.

func remove(Any, in: NSRange)

Removes all occurrences within a specified range in the array of a given object.

func removeObject(at: Int)

Removes the object at `index` .

func removeObjects(at: IndexSet)

Removes the objects at the specified indexes from the array.

func removeObject(identicalTo: Any)

Removes all occurrences of a given object in the array.

func removeObject(identicalTo: Any, in: NSRange)

Removes all occurrences of `anObject` within the specified range in the array.

func removeObjects(fromIndices: UnsafeMutablePointer&lt;Int>, numIndices: Int)

Removes the specified number of objects from the array, beginning at the specified index.

Deprecated

func removeObjects(in: [Any])

Removes from the receiving array the objects in another given array.

func removeObjects(in: NSRange)

Removes from the array each of the objects within a given range.

### Replacing Objects

func replaceObject(at: Int, with: Any)

Replaces the object at `index` with `anObject`.

func replaceObjects(at: IndexSet, with: [Any])

Replaces the objects in the receiving array at locations specified with the objects from a given array.

func replaceObjects(in: NSRange, withObjectsFrom: [Any], range: NSRange)

Replaces the objects in the receiving array specified by one given range with the objects in another array specified by another range.

func replaceObjects(in: NSRange, withObjectsFrom: [Any])

Replaces the objects in the receiving array specified by a given range with all of the objects from a given array.

func setArray([Any])

Sets the receiving array’s elements to those in another given array.

### Filtering Content

func filter(using: NSPredicate)

Evaluates a given predicate against the array’s content and leaves only objects that match.

### Rearranging Content

func exchangeObject(at: Int, withObjectAt: Int)

Exchanges the objects in the array at given indexes.

func sort(using: [NSSortDescriptor])

Sorts the receiver using a given array of sort descriptors.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the comparison method specified by a given Comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the receiver in ascending order using the specified options and the comparison method specified by a given Comparator block.

func sort((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver in ascending order as defined by the comparison function `compare`.

func sort(using: Selector)

Sorts the receiver in ascending order, as determined by the comparison method specified by a given selector.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSArray

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

