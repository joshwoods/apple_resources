

- Foundation
- NSCountedSet
-  init(capacity:) 

Initializer

# init(capacity:)

Returns a counted set object initialized with enough memory to hold a given number of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(capacity numItems: Int)
```

## Parameters 

`numItems`  

The initial capacity of the new counted set.

## Return Value

A counted set object initialized with enough memory to hold `numItems` objects

## Discussion

The method is the designated initializer for NSCountedSet.

Note that the capacity is simply a hint to help initial memory allocation—the initial count of the object is `0`, and the set still grows and shrinks as you add and remove objects. The hint is typically useful if the set will become large.

## See Also

### Related Documentation

init(capacity: Int)

Returns an initialized mutable set with a given initial capacity.

### Initializing a Counted Set

convenience init(array: [Any])

Returns a counted set object initialized with the contents of a given array.

convenience init(set: Set&lt;AnyHashable>)

Returns a counted set object initialized with the contents of a given set.

