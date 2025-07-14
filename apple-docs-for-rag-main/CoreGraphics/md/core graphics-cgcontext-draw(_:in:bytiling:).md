

- Core Graphics
- CGContext
-  draw(\_:in:byTiling:) 

Instance Method

# draw(\_:in:byTiling:)

Draws an image in the specified area.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func draw(
    _ image: CGImage,
    in rect: CGRect,
    byTiling: Bool = false
)
```

## Parameters 

`image`  

The image to draw.

`rect`  

The rectangle, in user space coordinates, in which to draw the image.

`byTiling`  

If true, this method fills the context’s entire clipping region by tiling many copies of the image, and the `rect` parameter defines the origin and size of the tiling pattern.

If false (the default), this method draws a single copy of the image in the area defined by the `rect` parameter.

## Discussion

This method scales the image (disproportionately, if necessary) to fit the bounds specified by the `rect` parameter.When the `byTiling` parameter is true, the image is tiled in user space—thus, unlike when drawing with patterns, the current transformation (see the ctm property) affects the final result.

## See Also

### Drawing Images and PDF Content

func drawPDFPage(CGPDFPage)

Draws the content of a PDF page into the current graphics context.

var interpolationQuality: CGInterpolationQuality

Returns the current level of interpolation quality for a graphics context.

enum CGInterpolationQuality

Levels of interpolation quality for rendering an image.

