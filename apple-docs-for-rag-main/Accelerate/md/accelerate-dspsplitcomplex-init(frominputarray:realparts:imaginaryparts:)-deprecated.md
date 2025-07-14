

- Accelerate
- DSPSplitComplex
-  init(fromInputArray:realParts:imaginaryParts:) Deprecated

Initializer

# init(fromInputArray:realParts:imaginaryParts:)

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    fromInputArray inputArray: [Float],
    realParts: inout [Float],
    imaginaryParts: inout [Float]
)
```

Deprecated

Use the `withUnsafeMutableBufferPointer` method on the real and imaginary arrays to create `DSPSplitComplex` for a defined scope.

