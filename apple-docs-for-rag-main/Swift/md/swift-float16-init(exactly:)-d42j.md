

- Swift
- Float16
-  init(exactly:) 

Initializer

# init(exactly:)

Creates a new instance from the given value, if it can be represented exactly.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(exactly value: Source) where Source : BinaryFloatingPoint
```

## Parameters 

`value`  

A floating-point value to be converted.

## Discussion

If the given floating-point value cannot be represented exactly, the result is `nil`.

