

- Foundation
- NSArray
-  index(of:inSortedRange:options:usingComparator:) 

Instance Method

# index(of:inSortedRange:options:usingComparator:)

Returns the index, within a specified range, of an object compared with elements in the array using a given `NSComparator` block.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(
    of obj: Any,
    inSortedRange r: NSRange,
    options opts: NSBinarySearchingOptions = [],
    usingComparator cmp: (Any, Any) -> ComparisonResult
) -> Int
```

## Parameters 

`obj`  

An object for which to search in the array.

If this value is `nil`, throws an invalidArgumentException.

`r`  

The range within the array to search for `obj`.

If `r` exceeds the bounds of the array (if the location plus length of the range is greater than the count of the array), throws an rangeException.

`opts`  

Options for the search. For possible values, see NSBinarySearchingOptions.

If you specify both firstEqual and lastEqual, throws an `NSInvalidArgumentException`.

`cmp`  

A comparator block used to compare the object `obj` with elements in the array.

If this value is `NULL`, throws an invalidArgumentException.

## Return Value

If the insertionIndex option is not specified:

- If the `obj` is found and neither firstEqual nor lastEqual is specified, returns an arbitrary matching object’s index.

- If the firstEqual option is also specified, returns the lowest index of equal objects.

- If the lastEqual option is also specified, returns the highest index of equal objects.

- If the object is not found, returns `NSNotFound`.

If the insertionIndex option is specified, returns the index at which you should insert `obj` in order to maintain a sorted array:

- If the `obj` is found and neither firstEqual nor lastEqual is specified, returns any equal or one larger index than any matching object’s index.

- If the firstEqual option is also specified, returns the lowest index of equal objects.

- If the lastEqual option is also specified, returns the highest index of equal objects.

- If the object is not found, returns the index of the least greater object, or the index at the end of the array if the object is larger than all other elements.

## Discussion

The elements in the array must have already been sorted using the comparator `cmp`. If the array is not sorted, the result is undefined.

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

func indexesOfObjects(options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes of objects in the array that pass a test in a given block for a given set of enumeration options.

func indexesOfObjects(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes, from a given set of indexes, of objects in the array that pass a test in a given block for a given set of enumeration options.

