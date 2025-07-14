

- Foundation
- NSArray
-  objectEnumerator() 

Instance Method

# objectEnumerator()

Returns an enumerator object that lets you access each object in the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectEnumerator() -> NSEnumerator
```

## Return Value

An enumerator object that lets you access each object in the array, in order, from the element at the lowest index upwards.

## Discussion

Returns an enumerator object that lets you access each object in the array, in order, starting with the element at index 0, as in:

```
NSEnumerator *enumerator = [myArray objectEnumerator];
id anObject;

while (anObject = [enumerator nextObject]) {
    /* code to act on each element as it is returned */
}
```

### Special Considerations

When you use this method with mutable subclasses of `NSArray`, you must not modify the array during enumeration.

It is more efficient to use the fast enumeration protocol (see NSFastEnumeration). Fast enumeration is available in macOS 10.5 and later and iOS 2.0 and later.

## See Also

### Related Documentation

func nextObject() -> Any?

Returns the next object from the collection being enumerated.

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

func objects(at: IndexSet) -> [Any]

Returns an array containing the objects in the array at the indexes specified by a given index set.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

