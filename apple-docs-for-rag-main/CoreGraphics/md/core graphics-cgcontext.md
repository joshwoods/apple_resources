

- Core Graphics
-  CGContext 

Class

# CGContext

A Quartz 2D drawing environment.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGContext
```

## Overview

A `CGContext` instance represents a Quartz 2D drawing destination. A graphics context contains drawing parameters and all device-specific information needed to render the paint on a page to the destination, whether the destination is a window in an application, a bitmap image, a PDF document, or a printer.

## Topics

### Creating Bitmap Graphics Contexts

init?(data: UnsafeMutableRawPointer?, width: Int, height: Int, bitsPerComponent: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: UInt32)

Creates a bitmap graphics context.

init?(data: UnsafeMutableRawPointer?, width: Int, height: Int, bitsPerComponent: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: UInt32, releaseCallback: CGBitmapContextReleaseDataCallback?, releaseInfo: UnsafeMutableRawPointer?)

Creates a bitmap graphics context with the specified callback function.

typealias CGBitmapContextReleaseDataCallback

A callback function used to release data associate with the bitmap context.

### Creating PDF Graphics Contexts

init?(CFURL, mediaBox: UnsafePointer&lt;CGRect>?, CFDictionary?)

Creates a URL-based PDF graphics context.

init?(consumer: CGDataConsumer, mediaBox: UnsafePointer&lt;CGRect>?, CFDictionary?)

Creates a PDF graphics context.

Auxiliary Dictionary Keys

Keys for the auxiliary info dictionary you specify when creating a PDF context.

### Converting Between Coordinate Spaces

var userSpaceToDeviceSpaceTransform: CGAffineTransform

Returns an affine transform that maps user space coordinates to device space coordinates.

func convertToDeviceSpace(CGPoint) -> CGPoint

Returns a point that is transformed from user space coordinates to device space coordinates.

func convertToUserSpace(CGPoint) -> CGPoint

Returns a point that is transformed from device space coordinates to user space coordinates.

func convertToDeviceSpace(CGRect) -> CGRect

Returns a rectangle that is transformed from user space coordinate to device space coordinates.

func convertToUserSpace(CGRect) -> CGRect

Returns a rectangle that is transformed from device space coordinate to user space coordinates.

func convertToDeviceSpace(CGSize) -> CGSize

Returns a size that is transformed from user space coordinates to device space coordinates.

func convertToUserSpace(CGSize) -> CGSize

Returns a size that is transformed from device space coordinates to user space coordinates.

### Constructing a Current Graphics Path

func beginPath()

Creates a new empty path in a graphics context.

func move(to: CGPoint)

Begins a new subpath at the specified point.

func addLine(to: CGPoint)

Appends a straight line segment from the current point to the specified point.

func addLines(between: [CGPoint])

Adds a sequence of connected straight-line segments to the current path.

func addRect(CGRect)

Adds a rectangular path to the current path.

func addRects([CGRect])

Adds a set of rectangular paths to the current path.

func addEllipse(in: CGRect)

Adds an ellipse that fits inside the specified rectangle.

func addArc(center: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Adds an arc of a circle to the current path, specified with a radius and angles.

func addArc(tangent1End: CGPoint, tangent2End: CGPoint, radius: CGFloat)

Adds an arc of a circle to the current path, specified with a radius and two tangent lines.

func addCurve(to: CGPoint, control1: CGPoint, control2: CGPoint)

Adds a cubic Bézier curve to the current path, with the specified end point and control points.

func addQuadCurve(to: CGPoint, control: CGPoint)

Adds a quadratic Bézier curve to the current path, with the specified end point and control point.

func addPath(CGPath)

Adds a previously created path object to the current path in a graphics context.

func closePath()

Closes and terminates the current path’s subpath.

var path: CGPath?

Returns a path object built from the current path information in a graphics context.

func replacePathWithStrokedPath()

Replaces the path in the graphics context with the stroked version of the path.

### Examining the Current Graphics Path

var boundingBoxOfPath: CGRect

Returns the smallest rectangle that contains the current path.

var currentPointOfPath: CGPoint

Returns the current point in a non-empty path.

var isPathEmpty: Bool

Indicates whether the current path contains any subpaths.

func pathContains(CGPoint, mode: CGPathDrawingMode) -> Bool

Checks to see whether the specified point is contained in the current path.

### Drawing the Current Graphics Path

func drawPath(using: CGPathDrawingMode)

Draws the current path using the provided drawing mode.

enum CGPathDrawingMode

Options for rendering a path.

func fillPath(using: CGPathFillRule)

Paints the area within the current path, as determined by the specified fill rule.

func strokePath()

Paints a line along the current path.

### Drawing Shapes

func clear(CGRect)

Paints a transparent rectangle.

func fill(CGRect)

Paints the area contained within the provided rectangle, using the fill color in the current graphics state.

func fill([CGRect])

Paints the areas contained within the provided rectangles, using the fill color in the current graphics state.

func fillEllipse(in: CGRect)

Paints the area of the ellipse that fits inside the provided rectangle, using the fill color in the current graphics state.

func stroke(CGRect)

Paints a rectangular path.

func stroke(CGRect, width: CGFloat)

Paints a rectangular path, using the specified line width.

func strokeEllipse(in: CGRect)

Strokes an ellipse that fits inside the specified rectangle.

func strokeLineSegments(between: [CGPoint])

Strokes a sequence of line segments.

### Drawing Images and PDF Content

func draw(CGImage, in: CGRect, byTiling: Bool)

Draws an image in the specified area.

func drawPDFPage(CGPDFPage)

Draws the content of a PDF page into the current graphics context.

var interpolationQuality: CGInterpolationQuality

Returns the current level of interpolation quality for a graphics context.

enum CGInterpolationQuality

Levels of interpolation quality for rendering an image.

### Drawing Gradients and Shadings

func drawLinearGradient(CGGradient, start: CGPoint, end: CGPoint, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the line defined by the provided starting and ending points.

func drawRadialGradient(CGGradient, startCenter: CGPoint, startRadius: CGFloat, endCenter: CGPoint, endRadius: CGFloat, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the area defined by the provided starting and ending circles.

struct CGGradientDrawingOptions

Drawing locations for gradients.

func drawShading(CGShading)

Fills the clipping path of a context with the specified shading.

### Drawing Text

var textMatrix: CGAffineTransform

Returns the current text matrix.

var textPosition: CGPoint

Returns the location at which text is drawn.

func selectFont(name: UnsafePointer&lt;CChar>, size: CGFloat, textEncoding: CGTextEncoding)

Sets the font and font size in a graphics context.

Deprecated

func setCharacterSpacing(CGFloat)

Sets the current character spacing.

func setFont(CGFont)

Sets the platform font in a graphics context.

func setFontSize(CGFloat)

Sets the current font size.

func setTextDrawingMode(CGTextDrawingMode)

Sets the current text drawing mode.

func setAllowsFontSmoothing(Bool)

Sets whether or not to allow font smoothing for a graphics context.

func setAllowsFontSubpixelPositioning(Bool)

Sets whether or not to allow subpixel positioning for a graphics context.

func setAllowsFontSubpixelQuantization(Bool)

Sets whether or not to allow subpixel quantization for a graphics context.

func setShouldSmoothFonts(Bool)

Enables or disables font smoothing in a graphics context.

func setShouldSubpixelPositionFonts(Bool)

Enables or disables subpixel positioning in a graphics context.

func setShouldSubpixelQuantizeFonts(Bool)

Enables or disables subpixel quantization in a graphics context.

func showGlyphs(g: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at the current text position.

Deprecated

func showGlyphs([CGGlyph], at: [CGPoint])

Draws a set of glyphs at a set of corresponding positions.

func showGlyphsAtPoint(x: CGFloat, y: CGFloat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int)

Displays an array of glyphs at a position you specify.

Deprecated

func showGlyphsWithAdvances(glyphs: UnsafePointer&lt;CGGlyph>?, advances: UnsafePointer&lt;CGSize>?, count: Int)

Draws an array of glyphs with varying offsets.

Deprecated

func showText(string: UnsafePointer&lt;CChar>, length: Int)

Displays a character array at the current text position, a point specified by the current text matrix.

Deprecated

func showTextAtPoint(x: CGFloat, y: CGFloat, string: UnsafePointer&lt;CChar>, length: Int)

Displays a character string at a position you specify.

Deprecated

enum CGTextDrawingMode

Modes for rendering text.

### Drawing Core Graphics Layers

func draw(CGLayer, at: CGPoint)

Draws the contents of a layer object at the specified point.

func draw(CGLayer, in: CGRect)

Draws the contents of a layer object into the specified rectangle.

### Setting Fill, Stroke, and Shadow Colors

func setFillColor(CGColor)

Sets the current fill color in a graphics context, using a CGColor.

func setFillColor(UnsafePointer&lt;CGFloat>)

Sets the current fill color.

func setFillColor(cyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceCMYK color space.

func setFillColor(gray: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceGray color space.

func setFillColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Sets the current fill color to a value in the DeviceRGB color space.

func setFillColorSpace(CGColorSpace)

Sets the fill color space in a graphics context.

func setShadow(offset: CGSize, blur: CGFloat)

Enables shadowing in a graphics context.

func setShadow(offset: CGSize, blur: CGFloat, color: CGColor?)

Enables shadowing with color a graphics context.

func setStrokeColor(CGColor)

Sets the current stroke color in a context, using a CGColor.

func setStrokeColor(UnsafePointer&lt;CGFloat>)

Sets the current stroke color.

func setStrokeColor(cyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceCMYK color space.

func setStrokeColor(gray: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceGray color space.

func setStrokeColor(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Sets the current stroke color to a value in the DeviceRGB color space.

func setStrokeColorSpace(CGColorSpace)

Sets the stroke color space in a graphics context.

func setStrokePattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the stroke pattern in the specified graphics context.

func setAlpha(CGFloat)

Sets the opacity level for objects drawn in a graphics context.

### Working with the Current Clipping Path

func clip(using: CGPathFillRule)

Modifies the current clipping path.

func clip(to: CGRect)

Sets the clipping path to the intersection of the current clipping path with the area defined by the specified rectangle.

func clip(to: [CGRect])

Sets the clipping path to the intersection of the current clipping path with the region defined by an array of rectangles.

func clip(to: CGRect, mask: CGImage)

Maps a mask into the specified rectangle and intersects it with the current clipping area of the graphics context.

var boundingBoxOfClipPath: CGRect

Returns the bounding box of a clipping path.

### Working with Transparency Layers

func beginTransparencyLayer(in: CGRect, auxiliaryInfo: CFDictionary?)

Begins a transparency layer whose contents are bounded by the specified rectangle.

func beginTransparencyLayer(auxiliaryInfo: CFDictionary?)

Begins a transparency layer.

func endTransparencyLayer()

Ends a transparency layer.

### Working with the Current Transformation Matrix

var ctm: CGAffineTransform

Returns the current transformation matrix.

func rotate(by: CGFloat)

Rotates the user coordinate system in a context.

func scaleBy(x: CGFloat, y: CGFloat)

Changes the scale of the user coordinate system in a context.

func translateBy(x: CGFloat, y: CGFloat)

Changes the origin of the user coordinate system in a context.

func concatenate(CGAffineTransform)

Transforms the user coordinate system in a context using a specified matrix.

### Setting Path Drawing Options

func setAllowsAntialiasing(Bool)

Sets whether or not to allow antialiasing for a graphics context.

func setFlatness(CGFloat)

Sets the accuracy of curved paths in a graphics context.

func setLineCap(CGLineCap)

Sets the style for the endpoints of lines drawn in a graphics context.

func setLineDash(phase: CGFloat, lengths: [CGFloat])

Sets the pattern for drawing dashed lines.

func setLineJoin(CGLineJoin)

Sets the style for the joins of connected lines in a graphics context.

func setLineWidth(CGFloat)

Sets the line width for a graphics context.

func setMiterLimit(CGFloat)

Sets the miter limit for the joins of connected lines in a graphics context.

func setPatternPhase(CGSize)

Sets the pattern phase of a context.

func setFillPattern(CGPattern, colorComponents: UnsafePointer&lt;CGFloat>)

Sets the fill pattern in the specified graphics context.

func setShouldAntialias(Bool)

Sets antialiasing on or off for a graphics context.

### Saving and Restoring Graphics State

func saveGState()

Pushes a copy of the current graphics state onto the graphics state stack for the context.

func restoreGState()

Sets the current graphics state to the state most recently saved.

### Managing a Graphics Context

func flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

func synchronize()

Marks a window context for update.

func setBlendMode(CGBlendMode)

Sets how sample values are composited by a graphics context.

enum CGBlendMode

Compositing operations for images.

func setRenderingIntent(CGColorRenderingIntent)

Sets the rendering intent in the current graphics state.

### Managing a Bitmap Graphics Context

These properties and methods are valid only when used with a `CGContext` object created with the initializers listed in Creating Bitmap Graphics Contexts.

var bitmapInfo: CGBitmapInfo

Obtains the bitmap information associated with a bitmap graphics context.

var alphaInfo: CGImageAlphaInfo

Returns the alpha information associated with the context, which indicates how a bitmap context handles the alpha component.

var bitsPerComponent: Int

Returns the bits per component of a bitmap context.

var bitsPerPixel: Int

Returns the bits per pixel of a bitmap context.

var bytesPerRow: Int

Returns the bytes per row of a bitmap context.

var colorSpace: CGColorSpace?

Returns the color space of a bitmap context.

var data: UnsafeMutableRawPointer?

Returns a pointer to the image data associated with a bitmap context.

var height: Int

Returns the height in pixels of a bitmap context.

var width: Int

Returns the width in pixels of a bitmap context.

func makeImage() -> CGImage?

Creates and returns a CGImage from the pixel data in a bitmap graphics context.

### Managing a PDF Graphics Context

These methods are valid only when used with a `CGContext` object created with the initializers listed in Creating PDF Graphics Contexts.

func beginPDFPage(CFDictionary?)

Begins a new page in a PDF graphics context.

func endPDFPage()

Ends the current page in the PDF graphics context.

func addDestination(CFString, at: CGPoint)

Sets a destination to jump to when a point in the current page of a PDF graphics context is clicked.

func setDestination(CFString, for: CGRect)

Sets a destination to jump to when a rectangle in the current PDF page is clicked.

func setURL(CFURL, for: CGRect)

Sets the URL associated with a rectangle in a PDF graphics context.

func addDocumentMetadata(CFData?)

Associates custom metadata with the PDF document.

func closePDF()

Closes a PDF document.

### Managing a Page-Based Graphics Context

func beginPage(mediaBox: UnsafePointer&lt;CGRect>?)

Starts a new page in a page-based graphics context.

func endPage()

Ends the current page in a page-based graphics context.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the type identifier for a graphics context.

### Constants

enum CGPathFillRule

Rules for determining which regions are interior to a path, used by the fillPath(using:) and clip(using:) methods.

enum CGTextEncoding

Text encodings for fonts.

### Instance Methods

func draw(CGImage, in: CGRect, by: CGToneMapping, options: CFDictionary?) -> Bool

func resetClip()

func setEDRTargetHeadroom(Float) -> Bool

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### 2D Drawing

class CGImage

A bitmap image or image mask.

class CGPath

An immutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

class CGMutablePath

A mutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

class CGLayer

An offscreen context for reusing content drawn with Core Graphics.

