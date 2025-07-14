

- Foundation
- NSHashTable
-  init(pointerFunctions:capacity:) 

Initializer

# init(pointerFunctions:capacity:)

Returns a hash table initialized with the given functions and capacity.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    pointerFunctions functions: NSPointerFunctions,
    capacity initialCapacity: Int
)
```

## Parameters 

`functions`  

The pointer functions for the new hash table.

`initialCapacity`  

The initial capacity of the hash table.

## Return Value

A hash table initialized with the given functions and capacity.

## Discussion

Hash tables allocate additional memory as needed, so `initialCapacity` simply establishes the object’s initial capacity.

## See Also

### Initialization

init(options: NSPointerFunctions.Options, capacity: Int)

Returns a hash table initialized with the given attributes.

