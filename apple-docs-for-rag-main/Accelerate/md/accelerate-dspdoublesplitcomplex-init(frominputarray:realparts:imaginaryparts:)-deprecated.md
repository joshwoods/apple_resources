

- Accelerate
- DSPDoubleSplitComplex
-  init(fromInputArray:realParts:imaginaryParts:) Deprecated

Initializer

# init(fromInputArray:realParts:imaginaryParts:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+visionOSwatchOS 6.0+tvOS 13.0+

``` source
init(
    fromInputArray inputArray: [Double],
    realParts: inout [Double],
    imaginaryParts: inout [Double]
)
```

Deprecated

Use the `withUnsafeMutableBufferPointer` method on the real and imaginary arrays to create `DSPSplitComplex` for a defined scope.

