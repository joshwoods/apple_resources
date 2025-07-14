

- Foundation
- NSIndexSet
-  index(in:options:passingTest:) 

Instance Method

# index(in:options:passingTest:)

Returns the index of the first object in the specified range that passes the predicate Block test.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(
    in range: NSRange,
    options opts: NSEnumerationOptions = [],
    passingTest predicate: (Int, UnsafeMutablePointer) -> Bool
) -> Int
```

## Parameters 

`range`  

The range of indexes to test.

`opts`  

A bitmask that specifies the options for the enumeration (whether it should be performed concurrently and whether it should be performed in reverse order). See NSEnumerationOptions for the supported values.

`predicate`  

The Block to apply to elements in the set.

The Block takes two arguments:

idx  
The index of the object.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this Boolean to YES within the Block.

The Block returns a Boolean value that indicates whether `obj` passed the test.

## Return Value

The index of the first object that passes the predicate test.

## See Also

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

func indexes(in: NSRange, options: NSEnumerationOptions, passingTest: (Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns an `NSIndexSet` containing the receiving index set’s objects in the specified range that pass the Block test.

