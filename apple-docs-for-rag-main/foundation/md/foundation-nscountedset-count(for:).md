

- Foundation
- NSCountedSet
-  count(for:) 

Instance Method

# count(for:)

Returns the count associated with a given object in the set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func count(for object: Any) -> Int
```

## Parameters 

`object`  

The object for which to return the count.

## Return Value

The count associated with `object` in the set, which can be thought of as the number of occurrences of `object` present in the set.

## See Also

### Related Documentation

var count: Int

The number of members in the set.

### Examining a Counted Set

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the set once, independent of its count.

