

- Swift
- DefaultStringInterpolation
-  init(literalCapacity:interpolationCount:) 

Initializer

# init(literalCapacity:interpolationCount:)

Creates a string interpolation with storage pre-sized for a literal with the indicated attributes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    literalCapacity: Int,
    interpolationCount: Int
)
```

## Discussion

Do not call this initializer directly. It is used by the compiler when interpreting string interpolations.

