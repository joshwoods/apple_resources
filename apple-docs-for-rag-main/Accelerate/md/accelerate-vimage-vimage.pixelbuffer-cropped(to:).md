

- Accelerate
- vImage
- vImage.PixelBuffer
-  cropped(to:) 

Instance Method

# cropped(to:)

Returns a new pixel buffer that contains a copy of the data specified as a subregion of an existing pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func cropped(to rect: CGRect) -> vImage.PixelBuffer
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`rect`  

A rectangle that specifies the portion of the image to keep.

## Return Value

A pixel buffer that contains of a copy of the specified subregion.

## Discussion

For example, the following code populates a pixel buffer from the center 3 x 3 pixels of a 5 x 5 planar buffer:

```
let src = vImage.PixelBuffer (
    pixelValues: [ 10, 11, 12, 13, 14,
                   20, 21, 22, 23, 24,
                   30, 31, 32, 33, 34,
                   40, 41, 42, 43, 44,
                   50, 51, 52, 53, 54 ],
    size: vImage.Size(width: 5,
                      height: 5))

let roi = CGRect(x: 1, y: 1,
                 width: 3, height: 3)

let dest = src.cropped(to: roi)

// Prints:
//  [ 21, 22, 23,
//    31, 32, 33,
//    41, 42, 43 ]
print(dest.array)
```

## See Also

### Cropping

func crop(at: CGPoint, destination: vImage.PixelBuffer&lt;Format>)

Crops the pixel buffer to a rectangle that’s defined by an origin and the destination buffer’s dimensions.

