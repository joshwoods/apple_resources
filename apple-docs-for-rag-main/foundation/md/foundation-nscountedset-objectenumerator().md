

- Foundation
- NSCountedSet
-  objectEnumerator() 

Instance Method

# objectEnumerator()

Returns an enumerator object that lets you access each object in the set once, independent of its count.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectEnumerator() -> NSEnumerator
```

## Return Value

An enumerator object that lets you access each object in the set once, independent of its count.

## Discussion

If you add a given object to the counted set multiple times, an enumeration of the set will produce that object only once.

You shouldn’t modify the set during enumeration. If you intend to modify the set, use the allObjects method to create a “snapshot,” then enumerate the snapshot and modify the original set.

## See Also

### Related Documentation

func nextObject() -> Any?

Returns the next object from the collection being enumerated.

### Examining a Counted Set

func count(for: Any) -> Int

Returns the count associated with a given object in the set.

