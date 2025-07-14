

- Accelerate
- vImage
- vImage.PixelBuffer
-  histogram() 

Instance Method

# histogram()

Calculates the histogram of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func histogram() -> vImage.PixelBuffer.Histogram8888
```

Available when `Format` is `vImage.Interleaved8x4`.

## Return Value

The histogram of the pixel buffer.

## See Also

### Related Documentation

func specifyHistogram(vImage.PixelBuffer&lt;Format>.Histogram8888, destination: vImage.PixelBuffer&lt;Format>)

Performs a histogram specification operation on an 8-bit-per-channel, 4-channel interleaved pixel buffer.

Specifying histograms with vImage

Calculate the histogram of one image, and apply it to a second image.

### Histogram calculation

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFFF

Calculates the histogram of a 32-bit-per-channel, 4-channel interleaved pixel buffer.

func histogram() -> vImage.PixelBuffer&lt;Format>.Histogram888

Calculates the histogram of an 8-bit-per-channel, 3-channel multiple-plane pixel buffer.

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFF

Calculates the histogram of a 32-bit-per-channel, 3-channel multiple-plane pixel buffer.

func histogram() -> vImage.PixelBuffer&lt;Format>.Histogram8888

Calculates the histogram of an 8-bit-per-channel, 4-channel multiple-plane pixel buffer.

func histogram(binCount: Int) -> vImage.PixelBuffer&lt;Format>.HistogramFFFF

Calculates the histogram of a 32-bit-per-channel, 4-channel multiple-plane pixel buffer.

