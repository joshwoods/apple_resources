

- Accelerate
- vImage_Buffer
-  rowBytes 

Instance Property

# rowBytes

The distance, in bytes, between the start of one pixel row and the next in an image, including any unused space between them.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rowBytes: Int
```

## Discussion

The rowBytes value must be at least the width multiplied by the pixel size, where the pixel size depends on the image format. You can provide a larger value, in which case the extra bytes extend beyond the end of each row of pixels. You may want to do this to improve performance, or to describe an image within a larger image without copying the data. The vImage library doesn’t treat the extra bytes as part of the image that the vImage buffer represents.

For example, the following code creates two buffers, `subBufferOne` and `subBufferTwo`, that point to the bottom-right quadrant of `bufferOne` and the top-left quadrant of `bufferTwo`, respectively. Note that both subbuffers share the same rowBytes as their original buffers.

```
let bufferOne = try vImage_Buffer(cgImage: cgImageOne,
                                  format: format)

let bufferTwo = try vImage_Buffer(cgImage: cgImageTwo,
                                  format: format)

// `subBufferTwo` points to the bottom-right quadrant of `bufferTwo`.
var start = (bufferTwo.rowBytes * Int(bufferOne.height / 2))    // y
start += Int(bufferOne.width / 2) * format.componentCount       // x
var subBufferOne = vImage_Buffer(data: bufferOne.data.advanced(by: start),
                                height: bufferOne.height / 2,
                                width: bufferOne.width / 2,
                                rowBytes: bufferTwo.rowBytes)

// `subBufferTwo` points to the top-left quadrant of `bufferTwo`.
let subBufferTwo = vImage_Buffer(data: bufferTwo.data,
                                height: bufferTwo.height / 2,
                                width: bufferTwo.width / 2,
                                rowBytes: bufferTwo.rowBytes)

try subBufferTwo.copy(destinationBuffer: &subBufferOne, pixelSize: 3)
```

On return, `bufferOne` contains the top-left quadrant of `bufferTwo` copied to its bottom-right quadrant.

When you allocate floating-point data for images, keep the data 4-byte-aligned by allocating bytes as integer multiples of four. For best performance, allocate bytes as integer multiples of 16.

## See Also

### Inspecting a buffer’s properties

var data: UnsafeMutableRawPointer!

A pointer to the top-left pixel of the image.

var height: vImagePixelCount

The height of the image, in pixels.

var width: vImagePixelCount

The width of the image, in pixels.

var size: CGSize

The size of the image, in pixels.

