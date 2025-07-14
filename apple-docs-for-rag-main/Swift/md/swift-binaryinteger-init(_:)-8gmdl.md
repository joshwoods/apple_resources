

- Swift
- BinaryInteger
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance from the given integer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ source: T) where T : BinaryInteger
```

**Required** Default implementations provided.

## Parameters 

`source`  

An integer to convert. `source` must be representable in this type.

## Discussion

If the value passed as `source` is not representable in this type, a runtime error may occur.

```
let x = -500 as Int
let y = Int32(x)
// y == -500

// -500 is not representable as a 'UInt32' instance
let z = UInt32(x)
// Error
```

## Default Implementations

### BinaryInteger Implementations

init?(String)

Creates a new integer value from the given string.

init&lt;T>(T)

init&lt;T>(T)

Creates a new instance from the given integer.

init&lt;T>(T)

Creates a new instance from the given integer.

## See Also

### Converting Integers

init&lt;T>(clamping: T)

Creates a new instance with the representable value that’s closest to the given integer.

**Required** Default implementation provided.

init&lt;T>(truncatingIfNeeded: T)

Creates a new instance from the bit pattern of the given instance by sign-extending or truncating to fit this type.

**Required** Default implementation provided.

