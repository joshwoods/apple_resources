

- Foundation
- NSMutableOrderedSet
-  init(capacity:) 

Initializer

# init(capacity:)

Returns an initialized mutable ordered set with a given initial capacity.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(capacity numItems: Int)
```

## Parameters 

`numItems`  

The initial capacity of the new ordered set.

## Return Value

An initialized mutable ordered set with initial capacity to hold `numItems` members.

## Discussion

Mutable ordered sets allocate additional memory as needed, so `numItems` simply establishes the set’s initial capacity.

This method is a designated initializer of `NSMutableOrderedSet`.

## See Also

### Creating a Mutable Ordered Set

init()

Initializes a newly allocated mutable ordered set.

