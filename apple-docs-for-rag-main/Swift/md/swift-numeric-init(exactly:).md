

- Swift
- Numeric
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance from the given integer, if it can be represented exactly.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly source: T) where T : BinaryInteger
```

**Required** Default implementations provided.

## Parameters 

`source`  

A value to convert to this type.

## Discussion

If the value passed as `source` is not representable exactly, the result is `nil`. In the following example, the constant `x` is successfully created from a value of `100`, while the attempt to initialize the constant `y` from `1_000` fails because the `Int8` type can represent `127` at maximum:

```
let x = Int8(exactly: 100)
// x == Optional(100)
let y = Int8(exactly: 1_000)
// y == nil
```

## Default Implementations

### BinaryFloatingPoint Implementations

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init?&lt;Source>(exactly: Source)

Creates a new instance from the given value, if it can be represented exactly.

### Numeric Implementations

init?&lt;T>(exactly: T)

init?&lt;T>(exactly: T)

init?&lt;T>(exactly: T)

