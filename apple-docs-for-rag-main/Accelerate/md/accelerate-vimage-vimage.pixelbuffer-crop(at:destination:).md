

- Accelerate
- vImage
- vImage.PixelBuffer
-  crop(at:destination:) 

Instance Method

# crop(at:destination:)

Crops the pixel buffer to a rectangle that’s defined by an origin and the destination buffer’s dimensions.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func crop(
    at origin: CGPoint,
    destination: vImage.PixelBuffer
)
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`origin`  

A point that specifies the origin of the image to keep.

`destination`  

The destination pixel buffer.

## Discussion

For example, the following code populates a pixel buffer from the center 3 x 3 pixels of a 5 x 5 planar buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [ 10, 11, 12, 13, 14,
                   20, 21, 22, 23, 24,
                   30, 31, 32, 33, 34,
                   40, 41, 42, 43, 44,
                   50, 51, 52, 53, 54 ],
    size: vImage.Size(width: 5,
                      height: 5))

let dest = vImage.PixelBuffer(
    size: vImage.Size(width: 3,
                      height: 3))

src.crop(at: CGPoint(x: 1, y: 1),
         destination: dest)

// Prints:
//  [ 21, 22, 23,
//    31, 32, 33,
//    41, 42, 43 ]
print(dest.array)
```

## See Also

### Cropping

func cropped(to: CGRect) -> vImage.PixelBuffer&lt;Format>

Returns a new pixel buffer that contains a copy of the data specified as a subregion of an existing pixel buffer.

