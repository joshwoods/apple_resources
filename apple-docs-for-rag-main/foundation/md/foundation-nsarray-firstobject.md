

- Foundation
- NSArray
-  firstObject 

Instance Property

# firstObject

The first object in the array.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var firstObject: Any? { get }
```

## Discussion

If the array is empty, returns `nil`.

## See Also

### Querying an Array

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the array.

var count: Int

The number of objects in the array.

var lastObject: Any?

The last object in the array.

func object(at: Int) -> Any

Returns the object located at the specified index.

subscript(Int) -> Any

Returns the object at the specified index.

func objects(at: IndexSet) -> [Any]

Returns an array containing the objects in the array at the indexes specified by a given index set.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

