

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(to:) 

Instance Method

# convert(to:)

Converts the contents of an 8-bit, four-plane pixel buffer to a four-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(to destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Planar8x4`.

## Parameters 

`destination`  

The destination pixel buffer.

## See Also

### Converting from 8-bit multiple plane to 8-bit interleaved

func convert(to: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Converts the contents of an 8-bit, three-plane pixel buffer to a three-channel interleaved pixel buffer.

