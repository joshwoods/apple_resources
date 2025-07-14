

- Foundation
- NSMutableData
-  init(length:) 

Initializer

# init(length:)

Initializes and returns a mutable data object containing a given number of zeroed bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(length: Int)
```

## Parameters 

`length`  

The number of bytes the object initially contains.

## Return Value

An initialized `NSMutableData` object containing `length` zeroed bytes.

## Discussion

The returned object has the same memory alignment guarantees as `malloc(_:)`.

## See Also

### Creating Mutable Data

init?(capacity: Int)

Returns an initialized mutable data object capable of holding the specified number of bytes.

