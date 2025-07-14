

- Accelerate
- vImage
- vImage.PixelBuffer
-  linearInterpolate(bufferB:interpolationConstant:destination:) 

Instance Method

# linearInterpolate(bufferB:interpolationConstant:destination:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func linearInterpolate(
    bufferB: vImage.PixelBuffer,
    interpolationConstant: Float,
    destination: vImage.PixelBuffer
)
```

Available when `Format` conforms to `StaticPixelFormat` and `Format.ComponentType` is `Float`.

