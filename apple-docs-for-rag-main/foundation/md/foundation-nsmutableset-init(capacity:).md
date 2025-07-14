

- Foundation
- NSMutableSet
-  init(capacity:) 

Initializer

# init(capacity:)

Returns an initialized mutable set with a given initial capacity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(capacity numItems: Int)
```

## Parameters 

`numItems`  

The initial capacity of the set.

## Return Value

An initialized mutable set with initial capacity to hold `numItems` members. The returned set might be different than the original receiver.

## Discussion

Mutable sets allocate additional memory as needed, so `numItems` simply establishes the object’s initial capacity.

This method is a designated initializer for `NSMutableSet`.

## See Also

### Creating a mutable set

init()

Initializes a newly allocated set.

