

- Swift
- Float16
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new value, if the given integer can be represented exactly.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(exactly value: Source) where Source : BinaryInteger
```

## Parameters 

`value`  

The integer to convert to a floating-point value.

## Discussion

If the given integer cannot be represented exactly, the result is `nil`.

