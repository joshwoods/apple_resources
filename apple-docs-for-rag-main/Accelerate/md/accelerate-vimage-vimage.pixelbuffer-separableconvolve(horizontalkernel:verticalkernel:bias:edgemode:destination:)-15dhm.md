

- Accelerate
- vImage
- vImage.PixelBuffer
-  separableConvolve(horizontalKernel:verticalKernel:bias:edgeMode:destination:) 

Instance Method

# separableConvolve(horizontalKernel:verticalKernel:bias:edgeMode:destination:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func separableConvolve(
    horizontalKernel: [Float],
    verticalKernel: [Float],
    bias: Float = 0,
    edgeMode: vImage.EdgeMode,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

