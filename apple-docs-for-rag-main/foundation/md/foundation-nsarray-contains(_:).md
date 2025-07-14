

- Foundation
- NSArray
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether a given object is present in the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ anObject: Any) -> Bool
```

## Parameters 

`anObject`  

An object to look for in the array.

## Return Value

true if `anObject` is present in the array, otherwise false.

## Discussion

Starting at index `0`, each element of the array is checked for equality with `anObject` until a match is found or the end of the array is reached. Objects are considered equal if isEqual(_:) returns true.

To determine if the array contains a particular instance of an object, you can test for identity rather than equality by calling the indexOfObjectIdentical(to:) method and comparing the return value to NSNotFound.

## See Also

### Related Documentation

func indexOfObjectIdentical(to: Any) -> Int

Returns the lowest index whose corresponding array value is identical to a given object.

func index(of: Any) -> Int

Returns the lowest index whose corresponding array value is equal to a given object.

### Querying an Array

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

func objects(at: IndexSet) -> [Any]

Returns an array containing the objects in the array at the indexes specified by a given index set.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

