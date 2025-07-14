

- Foundation
- NSOrderedSet
-  indexes(options:ofObjectsPassingTest:) 

Instance Method

# indexes(options:ofObjectsPassingTest:)

Returns the index of an object in the ordered set that passes a test in a given block for a given set of enumeration options.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func indexes(
    options opts: NSEnumerationOptions = [],
    ofObjectsPassingTest predicate: (Any, Int, UnsafeMutablePointer) -> Bool
) -> IndexSet
```

## Parameters 

`opts`  

A bitmask that specifies the options for the enumeration (whether it should be performed concurrently and whether it should be performed in reverse order).

`predicate`  

The block to apply to elements in the ordered set.

The block takes three arguments:

obj  
The element in the ordered set.

Term  
The index of the element in the ordered set.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this value to true within the block.

## Return Value

The index whose corresponding value in the ordered set passes the test specified by `predicate` and `opts`. If the `opts` bitmask specifies reverse order, then the last item that matches is returned. Otherwise, the index of the first matching object is returned. If no objects in the ordered set pass the test, returns `NSNotFound`.

## Discussion

By default, the enumeration starts with the first object and continues serially through the ordered set to the last object. You can specify concurrent and/or reverse as enumeration options to modify this behavior.

Important

If the block parameter or `s` is `nil`, this method raises an exception.

## See Also

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

