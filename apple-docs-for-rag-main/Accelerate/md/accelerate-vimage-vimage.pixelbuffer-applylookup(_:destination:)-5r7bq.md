

- Accelerate
- vImage
- vImage.PixelBuffer
-  applyLookup(\_:destination:) 

Instance Method

# applyLookup(\_:destination:)

Applies a lookup table to transform an 8-bit planar image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func applyLookup(
    _ lookupTable: [Pixel_8],
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Planar8`.

## Parameters 

`lookupTable`  

A lookup table that contains 256 Pixel_8888 ARGB values. The function discards the alpha component.

`destination`  

The destination pixel buffer.

## Discussion

You can use this function to create custom response curves (that is, the value of an output pixel based on the value of the corresponding input pixel). Changing the shape of the response curve changes the brightness and contrast of an image.

The following code creates a simple lookup table that’s based on a sigmoid function. This example uses BNNS to create 256 `Float` values in the range `0...1` that describe a sigmoid curve. The code scales the sigmoid curve values to `0...255` and returns Pixel_8 values that are suitable for use as a lookup table.

```
let count = 256

// The following code populates the array descriptor with sigmoid
// curve values in the range 0...1:
let sigmoidSourceValues: [Float] = vDSP.ramp(in: -10 ... 10,
                                             count: count)
let descriptor = BNNSNDArrayDescriptor.allocate(initializingFrom: sigmoidSourceValues,
                                                shape: .vector(count))
defer {
    descriptor.deallocate()
}
let activationLayer = BNNS.ActivationLayer(function: .sigmoid,
                                           input: descriptor,
                                           output: descriptor,
                                           filterParameters: nil)
try? activationLayer!.apply(batchSize: 1,
                            input: descriptor,
                            output: descriptor)

let lookup = descriptor.data!.withMemoryRebound(to: Float.self,
                                                   capacity: count) {
    // Create an `UnsafeMutableBufferPointer` from the descriptor data.
    var sigmoid = UnsafeMutableBufferPointer(start: $0,
                                             count: count)

    // Scale the sigmoid values from 0...1 to 0...255.
    vDSP.multiply(255.0,
                  sigmoid,
                  result: &sigmoid)

    // Create Pixel_8 values from the Float sigmoid values.
    return vDSP.floatingPointToInteger(sigmoid,
                                       integerType: Pixel_8.self,
                                       rounding: .towardNearestInteger)
}
```

The graph below visualizes the values in the lookup table:

Use the following code to apply the lookup table to a vImage.Planar8 source buffer and write the result to a vImage.Planar8 destination buffer:

```
let destinationBuffer = vImage.PixelBuffer(
    size: sourceBuffer.size,
    pixelFormat: vImage.Planar8.self)

sourceBuffer.applyLookup(lookup, destination: destinationBuffer)
```

The images below show an example grayscale source image on the left and the transformed result on the right. The operation flattens the response for very dark and very bright areas and increases the contrast in the destination image.

## See Also

### Transforming with a lookup table

func applyLookup([Pixel_F], destination: vImage.PixelBuffer&lt;vImage.PlanarF>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func applyLookup([Pixel_16U], destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Applies a lookup table to transform an 8-bit planar image to a 16-bit planar image.

func applyLookup([Pixel_8888], destination: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Applies a lookup table to transform an 8-bit planar image to an 8-bit-per-channel, three-channel interleaved image.

func applyLookup([Pixel_FFFF], destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Applies a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, three-channel interleaved image.

func applyLookup(alphaTable: [Pixel_8]?, redTable: [Pixel_8]?, greenTable: [Pixel_8]?, blueTable: [Pixel_8]?, destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Applies a set of four lookup tables to transform an interleaved, four-channel 8-bit image.

