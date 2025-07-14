

- Accelerate
- vImage
- vImage.PixelBuffer
-  convolve(with:bias:edgeMode:destination:) 

Instance Method

# convolve(with:bias:edgeMode:destination:)

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func convolve(
    with kernel: vImage.ConvolutionKernel2D,
    bias: Float? = nil,
    edgeMode: vImage.EdgeMode,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

