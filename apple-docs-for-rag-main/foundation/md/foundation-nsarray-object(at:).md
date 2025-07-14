

- Foundation
- NSArray
-  object(at:) 

Instance Method

# object(at:)

Returns the object located at the specified index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(at index: Int) -> Any
```

## Parameters 

`index`  

An index within the bounds of the array.

## Return Value

The object located at `index`.

## Discussion

If `index` is beyond the end of the array (that is, if `index` is greater than or equal to the value returned by `count`), an rangeException is raised.

## See Also

### Querying an Array

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the array.

var count: Int

The number of objects in the array.

var firstObject: Any?

The first object in the array.

var lastObject: Any?

The last object in the array.

subscript(Int) -> Any

Returns the object at the specified index.

func objects(at: IndexSet) -> [Any]

Returns an array containing the objects in the array at the indexes specified by a given index set.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

