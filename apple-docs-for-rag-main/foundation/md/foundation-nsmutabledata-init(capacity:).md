

- Foundation
- NSMutableData
-  init(capacity:) 

Initializer

# init(capacity:)

Returns an initialized mutable data object capable of holding the specified number of bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(capacity: Int)
```

## Parameters 

`capacity`  

The number of bytes the data object can initially contain.

## Return Value

An initialized `NSMutableData` object capable of holding `capacity` bytes.

## Discussion

The returned object has the same memory alignment guarantees as `malloc(_:)`.

This method doesn’t necessarily allocate the requested memory right away. Mutable data objects allocate additional memory as needed, so `capacity` simply establishes the object’s initial capacity. When it does allocate the initial memory, though, it allocates the specified amount. This method sets the length of the data object to `0`.

If the capacity specified in `capacity` is greater than four memory pages in size, this method may round the amount of requested memory up to the nearest full page.

## See Also

### Creating Mutable Data

init?(length: Int)

Initializes and returns a mutable data object containing a given number of zeroed bytes.

