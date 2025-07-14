

- Swift
- BinaryFloatingPoint
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance from the given value, rounded to the closest possible representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ value: Source) where Source : BinaryFloatingPoint
```

**Required** Default implementations provided.

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

## Default Implementations

### BinaryFloatingPoint Implementations

init&lt;Source>(Source)

Creates a new instance from the given value, rounded to the closest possible representation.

init&lt;Source>(Source)

Creates a new value, rounded to the closest possible representation.

## See Also

### Converting Floating-Point Values

init(Float)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

init(Double)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

init(Float80)

Creates a new instance from the given value, rounded to the closest possible representation.

**Required** Default implementations provided.

