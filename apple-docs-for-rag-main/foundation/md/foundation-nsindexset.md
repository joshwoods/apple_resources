

- Foundation
-  NSIndexSet 

Class

# NSIndexSet

An immutable collection of unique integer values that represent indexes in another collection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSIndexSet
```

## Mentioned in 

init

## Overview

In Swift, this type bridges to IndexSet; use NSIndexSet when you need reference semantics or other Foundation-specific behavior.

The `NSIndexSet` class represents an immutable collection of unique unsigned integers, known as **indexes** because of the way they are used. This collection is referred to as an **index set**. Indexes must be in the range `0 .. NSNotFound - 1`.

You use index sets in your code to store indexes into some other data structure. For example, given an `NSArray` object, you could use an index set to identify a subset of objects in that array.

You should not use index sets to store an arbitrary collection of integer values because index sets store indexes as sorted ranges. This makes them more efficient than storing a collection of individual integers. It also means that each index value can only appear once in the index set.

The designated initializers of the `NSIndexSet` class are: doc:nsindexset/1807255-init, init(indexesIn:), and init(indexSet:).

You must not subclass the `NSIndexSet` class.

The mutable subclass of `NSIndexSet` is NSMutableIndexSet.

Important

The Swift overlay to the Foundation framework provides the IndexSet structure, which bridges to the NSIndexSet class and its mutable subclass, NSMutableIndexSet. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating Index Sets

convenience init(index: Int)

Initializes an allocated NSIndexSet object with an index.

init(indexesIn: NSRange)

Initializes an allocated NSIndexSet object with an index range.

init(indexSet: IndexSet)

Initializes an allocated NSIndexSet object with an index set.

### Querying Index Sets

func contains(Int) -> Bool

Indicates whether the index set contains a specific index.

func contains(IndexSet) -> Bool

Indicates whether the receiving index set contains a superset of the indexes in another index set.

func contains(in: NSRange) -> Bool

Indicates whether the index set contains the indexes represented by an index range.

func intersects(in: NSRange) -> Bool

Indicates whether the index set contains any of the indexes in a range.

var count: Int

The number of indexes in the index set.

func countOfIndexes(in: NSRange) -> Int

Returns the number of indexes in the index set that are members of a given range.

func index(passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the first object that passes the predicate Block test.

func indexes(passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns an `NSIndexSet` containing the receiving index set’s objects that pass the Block test.

func index(options: NSEnumerationOptions, passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the first object that passes the predicate Block test using the specified enumeration options.

func indexes(options: NSEnumerationOptions, passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns an `NSIndexSet` containing the receiving index set’s objects that pass the Block test using the specified enumeration options.

func index(in: NSRange, options: NSEnumerationOptions, passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the first object in the specified range that passes the predicate Block test.

func indexes(in: NSRange, options: NSEnumerationOptions, passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns an `NSIndexSet` containing the receiving index set’s objects in the specified range that pass the Block test.

### Enumerating Index Set Content

func enumerateRanges(in: NSRange, options: NSEnumerationOptions, using: (NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over the ranges in the range of objects using the block

func enumerateRanges((NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the index set, in the specified ranges.

func enumerateRanges(options: NSEnumerationOptions, using: (NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the index set, in the specified ranges.

### Comparing Index Sets

func isEqual(to: IndexSet) -> Bool

Indicates whether the indexes in the receiving index set are the same indexes contained in another index set.

### Getting Indexes

var firstIndex: Int

The first index in the index set.

var lastIndex: Int

The last index in the index set.

func indexLessThanIndex(Int) -> Int

Returns either the closest index in the index set that is less than a specific index or the not-found indicator.

func indexLessThanOrEqual(to: Int) -> Int

Returns either the closest index in the index set that is less than or equal to a specific index or the not-found indicator.

func indexGreaterThanOrEqual(to: Int) -> Int

Returns either the closest index in the index set that is greater than or equal to a specific index or the not-found indicator.

func indexGreaterThanIndex(Int) -> Int

Returns either the closest index in the index set that is greater than a specific index or the not-found indicator.

func getIndexes(UnsafeMutablePointer&lt;Int>, maxCount: Int, inIndexRange: NSRangePointer?) -> Int

The index set fills an index buffer with the indexes contained both in the index set and in an index range, returning the number of indexes copied.

### Enumerating Indexes

func enumerate((Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block using each object in the index set.

func enumerate(options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block over the index set’s indexes, using the specified enumeration options.

func enumerate(in: NSRange, options: NSEnumerationOptions, using: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given Block using the indexes in the specified range, using the specified enumeration options.

func makeIterator() -> NSIndexSetIterator

Returns an *iterator* over the elements of this *sequence*.

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

### Default Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableIndexSet

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

