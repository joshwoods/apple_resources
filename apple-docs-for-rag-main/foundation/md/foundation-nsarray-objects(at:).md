

- Foundation
- NSArray
-  objects(at:) 

Instance Method

# objects(at:)

Returns an array containing the objects in the array at the indexes specified by a given index set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objects(at indexes: IndexSet) -> [Any]
```

## Return Value

An array containing the objects in the array at the indexes specified by `indexes`.

## Discussion

The returned objects are in the ascending order of their indexes in `indexes`, so that object in returned array with higher index in indexes will follow the object with smaller index in `indexes`.

Raises an rangeException if any location in `indexes` exceeds the bounds of the array, `indexes` is `nil`.

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

func object(at: Int) -> Any

Returns the object located at the specified index.

subscript(Int) -> Any

Returns the object at the specified index.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

