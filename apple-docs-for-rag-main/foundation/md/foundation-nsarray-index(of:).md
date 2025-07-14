

- Foundation
- NSArray
-  index(of:) 

Instance Method

# index(of:)

Returns the lowest index whose corresponding array value is equal to a given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(of anObject: Any) -> Int
```

## Parameters 

`anObject`  

An object.

## Return Value

The lowest index whose corresponding array value is equal to `anObject`. If none of the objects in the array is equal to `anObject`, returns `NSNotFound`.

## Discussion

Starting at index `0`, each element of the array is passed as an argument to an isEqual(_:) message sent to `anObject` until a match is found or the end of the array is reached. Objects are considered equal if isEqual(_:) (declared in the NSObjectProtocol protocol) returns true.

## See Also

### Related Documentation

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the array.

### Finding Objects in an Array

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

func indexesOfObjects(options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes of objects in the array that pass a test in a given block for a given set of enumeration options.

func indexesOfObjects(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes, from a given set of indexes, of objects in the array that pass a test in a given block for a given set of enumeration options.

func index(of: Any, inSortedRange: NSRange, options: NSBinarySearchingOptions, usingComparator: (Any, Any) -> ComparisonResult) -> Int

Returns the index, within a specified range, of an object compared with elements in the array using a given `NSComparator` block.

