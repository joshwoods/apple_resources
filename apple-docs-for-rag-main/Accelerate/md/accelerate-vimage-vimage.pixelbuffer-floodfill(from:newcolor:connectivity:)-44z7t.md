

- Accelerate
- vImage
- vImage.PixelBuffer
-  floodFill(from:newColor:connectivity:) 

Instance Method

# floodFill(from:newColor:connectivity:)

Applies an in-place flood-fill operation to the 8-bit planar image.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func floodFill(
    from seed: CGPoint,
    newColor: Pixel_8,
    connectivity: vImage.FloodFillConnectivity
)
```

Available when `Format` is `vImage.Planar8`.

## Parameters 

`seed`  

The coordinates that define the position of the seed pixel inside the connected component.

`newColor`  

The new pixel value that overwrites the pixels in the connected component.

`connectivity`  

An enumeration that specifies which pixels the operation includes as neighbors. Pass vImage.FloodFillConnectivity.edges to specify a four-connected neighborhood of a pixel that includes the pixels to the left and right, and those above and below. Pass vImage.FloodFillConnectivity.edgesAndCorners to specify an eight-connected neighborhood that includes the four-connected neighborhood and the pixels on the four diagonals.

## Discussion

The flood-fill function sets all pixels that are neighboring and identical to the seed pixel to a new color. The operation continues until it reaches the image boundary or until it sets all pixels within the connected component to the new value.

The following code applies a flood fill to an 8-bit planar pixel buffer and uses the image’s center pixel as the seed.

```
// `pixelBuffer` is a `vImage.PixelBuffer`.

pixelBuffer.floodFill(from: CGPoint(x: pixelBuffer.width / 2,
                                    y: pixelBuffer.height / 2),
                      newColor: fillColor,
                      connectivity: .edgesAndCorners)
```

The image below shows the original line-art image on the left, and the flood-filled image on the right:

## See Also

### Related Documentation

Applying flood fills to an image

Fill consistently colored connected parts of an image with a new color.

### Applying a flood fill to an image

func floodFill(from: CGPoint, newColor: Pixel_8888, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the interleaved 4-channel, 8-bit-per-pixel image.

func floodFill(from: CGPoint, newColor: Pixel_16U, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the unsigned 16-bit planar image.

func floodFill(from: CGPoint, newColor: Pixel_ARGB_16U, connectivity: vImage.FloodFillConnectivity)

Applies an in-place flood-fill operation to the interleaved 4-channel, unsigned16-bit-per-pixel image.

