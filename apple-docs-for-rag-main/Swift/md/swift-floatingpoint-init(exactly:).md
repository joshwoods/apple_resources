

- Swift
- FloatingPoint
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new value, if the given integer can be represented exactly.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly value: Source) where Source : BinaryInteger
```

**Required** Default implementations provided.

## Parameters 

`value`  

The integer to convert to a floating-point value.

## Discussion

If the given integer cannot be represented exactly, the result is `nil`.

## Default Implementations

### BinaryFloatingPoint Implementations

init?&lt;Source>(exactly: Source)

Creates a new value, if the given integer can be represented exactly.

init?&lt;Source>(exactly: Source)

Creates a new instance from the given value, if it can be represented exactly.

