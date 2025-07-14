

- Core Graphics
- CGContext
-  drawPDFPage(\_:) 

Instance Method

# drawPDFPage(\_:)

Draws the content of a PDF page into the current graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func drawPDFPage(_ page: CGPDFPage)
```

## Parameters 

`page`  

A Core Graphics PDF page.

## Discussion

This function works in conjunction with the CGPDFPage type to draw individual PDF pages into a context.

## See Also

### Drawing Images and PDF Content

func draw(CGImage, in: CGRect, byTiling: Bool)

Draws an image in the specified area.

var interpolationQuality: CGInterpolationQuality

Returns the current level of interpolation quality for a graphics context.

enum CGInterpolationQuality

Levels of interpolation quality for rendering an image.

