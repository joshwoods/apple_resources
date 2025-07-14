

- Core Graphics
- CGContext
-  interpolationQuality 

Instance Property

# interpolationQuality

Returns the current level of interpolation quality for a graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var interpolationQuality: CGInterpolationQuality { get set }
```

## Discussion

Interpolation quality is a graphics state parameter that provides a hint for the level of quality to use for image interpolation (for example, when scaling the image). Not all contexts support all interpolation quality levels.

## See Also

### Drawing Images and PDF Content

func draw(CGImage, in: CGRect, byTiling: Bool)

Draws an image in the specified area.

func drawPDFPage(CGPDFPage)

Draws the content of a PDF page into the current graphics context.

enum CGInterpolationQuality

Levels of interpolation quality for rendering an image.

