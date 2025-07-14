

- Foundation
- NSIndexSet
-  countOfIndexes(in:) 

Instance Method

# countOfIndexes(in:)

Returns the number of indexes in the index set that are members of a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func countOfIndexes(in range: NSRange) -> Int
```

## Parameters 

`range`  

Index range being inquired about.

## Return Value

Number of indexes in the index set that are members of `indexRange`.

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

