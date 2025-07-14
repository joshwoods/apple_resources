

- Foundation
- NSHashTable
-  init(options:capacity:) 

Initializer

# init(options:capacity:)

Returns a hash table initialized with the given attributes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    options: NSPointerFunctions.Options = [],
    capacity initialCapacity: Int
)
```

## Parameters 

`options`  

A bit field that specifies the options for the elements in the hash table. For possible values, see NSHashTableOptions.

`initialCapacity`  

The initial number of elements the hash table can hold.

## Return Value

A hash table initialized with options specified by `options` and initial capacity of `capacity`.

## See Also

### Related Documentation

Collections Programming Topics

### Initialization

init(pointerFunctions: NSPointerFunctions, capacity: Int)

Returns a hash table initialized with the given functions and capacity.

