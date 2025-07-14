

- Swift
- Array
-  init(fromSplitComplex:scale:count:) 

Initializer

# init(fromSplitComplex:scale:count:)

Creates a new array of single-precision values from a `DSPDoubleSplitComplex` structure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    fromSplitComplex splitComplex: DSPDoubleSplitComplex,
    scale: Double,
    count: Int
)
```

Available when `Element` is `Double`.

## Parameters 

`scale`  

A multiplier to apply during conversion.

`count`  

The length of the required resulting array (typically half the count of either the real or imaginary parts of the `DSPSplitComplex`.

