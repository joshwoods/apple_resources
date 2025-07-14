

- Foundation
- NSOrderedSet
-  enumerateObjects(options:using:) 

Instance Method

# enumerateObjects(options:using:)

Executes a given block using each object in the set, using the specified enumeration options.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateObjects(
    options opts: NSEnumerationOptions = [],
    using block: (Any, Int, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`opts`  

A bitmask that specifies the options for the enumeration (whether it should be performed concurrently and whether it should be performed in reverse order).

`block`  

The block to apply to elements in the ordered set.

The block takes three arguments:

obj  
The element in the set.

idx  
The index of the item in the set.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this value to true within the block.

The block returns a Boolean value that indicates whether `obj` passed the test.

## See Also

### Accessing Set Members

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the ordered set.

func enumerateObjects(at: IndexSet, options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using the objects in the ordered set at the specified indexes.

func enumerateObjects((Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the ordered set.

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

