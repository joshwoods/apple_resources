

- Foundation
- NSArray
-  indexesOfObjects(options:passingTest:) 

Instance Method

# indexesOfObjects(options:passingTest:)

Returns the indexes of objects in the array that pass a test in a given block for a given set of enumeration options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func indexesOfObjects(
    options opts: NSEnumerationOptions = [],
    passingTest predicate: (Any, Int, UnsafeMutablePointer) -> Bool
) -> IndexSet
```

## Parameters 

`opts`  

A bit mask that specifies the options for the enumeration (whether it should be performed concurrently and whether it should be performed in reverse order).

`predicate`  

The block to apply to elements in the array.

The block takes three arguments:

obj  
The element in the array.

idx  
The index of the element in the array.

stop  
A reference to a Boolean value. The block can set the value to true to stop further enumeration of the array. If a block stops further enumeration, that block continues to run until it’s finished. When the `NSEnumerationConcurrent` enumeration option is specified, enumeration stops after all of the currently running blocks finish. The `stop` argument is an out-only argument. You should only ever set this Boolean to true within the block.

The block returns a Boolean value that indicates whether `obj` passed the test.

## Return Value

The indexes whose corresponding values in the array pass the test specified by `predicate`. If no objects in the array pass the test, returns an empty index set.

## Discussion

By default, the enumeration starts with the first object and continues serially through the array to the last object. You can specify concurrent and/or reverse as enumeration options to modify this behavior.

Important

If the block parameter is `nil` this method will raise an exception.

## See Also

### Finding Objects in an Array

func index(of: Any) -> Int

Returns the lowest index whose corresponding array value is equal to a given object.

func index(of: Any, in: NSRange) -> Int

Returns the lowest index within a specified range whose corresponding array value is equal to a given object .

func indexOfObjectIdentical(to: Any) -> Int

Returns the lowest index whose corresponding array value is identical to a given object.

func indexOfObjectIdentical(to: Any, in: NSRange) -> Int

Returns the lowest index within a specified range whose corresponding array value is equal to a given object .

func indexOfObject(passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the first object in the array that passes a test in a given block.

func indexOfObject(options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of an object in the array that passes a test in a given block for a given set of enumeration options.

func indexOfObject(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index, from a given set of indexes, of the first object in the array that passes a test in a given block for a given set of enumeration options.

func indexesOfObjects(passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes of objects in the array that pass a test in a given block.

func indexesOfObjects(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes, from a given set of indexes, of objects in the array that pass a test in a given block for a given set of enumeration options.

func index(of: Any, inSortedRange: NSRange, options: NSBinarySearchingOptions, usingComparator: (Any, Any) -> ComparisonResult) -> Int

Returns the index, within a specified range, of an object compared with elements in the array using a given `NSComparator` block.

