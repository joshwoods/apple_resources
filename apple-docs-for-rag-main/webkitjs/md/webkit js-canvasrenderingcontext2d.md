

- WebKit JS
-  CanvasRenderingContext2D 

Class

# CanvasRenderingContext2D

The `CanvasRenderingContext2D` class provides a 2D drawing context for a canvas element. Use the methods of this class to draw on the canvas. To obtain an instance of the `CanvasRenderingContext2D`, call the `getContext('2d')` method on a canvas object. See Safari HTML5 Canvas Guide for usage examples.

Safari Desktop 10.0+Safari Mobile 1.0+

``` source
interface CanvasRenderingContext2D
```

## Topics

### Drawing Rectangles

clearRect

Clears the specified rectangle to transparent black—RGBa(0,0,0,0).

fillRect

Fills a specified rectangle in the current fill color, gradient, or pattern.

strokeRect

Draws a rectangle using the current stroke color, pattern, or gradient.

### Creating Paths (Lines, Curves, Arcs, and Shapes)

Paths are made up of line segments, curves, and arcs. A path is drawn when you call the `fill()` or `stroke()` methods.

beginPath

Denotes the beginning of new path.

clip

Constrains the clipping region of the canvas to the current path.

isPointInPath

Determines whether a specified point is within the area defined by the current path.

### Filling and Stroking Lines and Paths

fill

Fills the current path using the current fill color, gradient, or pattern.

fillStyle

A CSS color, a gradient, or a pattern used to fill shapes and text.

lineCap

A string specifying the type of end cap to put on lines to be drawn using `lineTo()`.

lineJoin

A string specifying the manner in which line joins are drawn.

lineWidth

A floating-point number that controls the width of lines and strokes, in pixels.

miterLimit

A floating-point number that controls the miter limit ratio for mitered line joins.

stroke

Draws the outline of the current path using the current stroke style and line width.

strokeStyle

A CSS color, a gradient, or a pattern used to stroke lines and shapes.

### Drawing Images

drawImage

Draws the specified image with its upper-left corner at the specified point on the canvas, optionally scaling the image to a specified width and height. Alternatively, draws a specified region of the image, mapped to a specified region of the canvas.

### Drawing Text

fillText

Draws a line of text at the specified x,y coordinates, optionally scaled to a specified maximum width.

font

A string containing font settings, such as the font family, size, and weight.

measureText

Determines the width of the bounding box required to render the specified text with the current font settings.

strokeText

Draws a line of text in outline at the specified x,y coordinates, optionally limited to a specified maximum width.

textAlign

A string that specifies whether text is left-justified, right-justified, or centered.

textBaseline

A string that specifies how the bounding box aligns vertically relative to the y-coordinate.

### Changing the Coordinate System

The current transformation matrix is applied to the canvas coordinate system. These methods modify the current transformation matrix.

rotate

Rotates the canvas coordinate system.

scale

Scales the canvas coordinate system horizontally and vertically.

setTransform

Sets the transformation matrix.

transform

Transforms the current transformation matrix using another matrix.

translate

Moves the origin of the canvas coordinate system.

### Saving and Restoring Settings

save

Saves the current context settings on the stack.

restore

Restores the last saved set of context settings.

### Compositing

globalAlpha

A floating-point number controlling the degree of opacity for all drawing operations.

globalCompositeOperation

A string representing the compositing method for drawing operations.

### Creating Gradients and Patterns

Gradients or patterns can be used instead of colors as the stroke or fill style.

createLinearGradient

Creates a linear gradient object with a specified start point and a specified end point.

createPattern

Creates a pattern object using the specified image as a template. The pattern can be specified as repeating horizontally, vertically, both horizontally and vertically (the default), or not at all.

createRadialGradient

Creates a radial gradient object using the cone defined by the specified starting and ending circles.

### Manipulating Pixels

createImageData

Creates an opaque object whose `data` property contains a one-dimensional array of pixel values, initialized to transparent black.

getImageData

Gets an `imageData` object containing an RGBa pixel array corresponding to a rectangular area of the canvas.

putImageData

Blits the contents of an `imageData` object to the canvas. Alternatively, blits a specified region of the `imageData` object to the canvas.

### Working with Shadows

If shadows are enabled, all `stroke()`, `fill()`, and `drawImage()` operations include a shadow. Shadows need not be turned on or off using a method. You can enable or disable shadows by setting the `shadowColor`, `shadowBlur`, `shadowOffsetX`, and `shadowOffsetY` properties.

clearShadow

Turns shadows off.

shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

shadowColor

A string that contains the RGBa color value of shadows.

shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

### Constants

Global Compositing Operation Constants

Constants used to set the `globalCompositeOperation` property.

textBaseline Constants

Constants used to set the `textBaseline` property that specify the vertical alignment of the bounding box relative to its y-coordinate.

textAlign Constants

Constants used with the `textAlign` property that specify the horizontal alignment of the bounding box relative to its x-coordinate.

### Instance Properties

canvas

direction

imageSmoothingEnabled

imageSmoothingQuality

lineDashOffset

webkitBackingStorePixelRatio

webkitImageSmoothingEnabled

webkitLineDash

webkitLineDashOffset

### Instance Methods

commit

drawFocusIfNeeded

drawImageFromRect

getLineDash

isPointInStroke

resetTransform

setAlpha

setCompositeOperation

setFillColor

setLineCap

setLineDash

setLineJoin

setLineWidth

setMiterLimit

setShadow

setStrokeColor

webkitGetImageDataHD

webkitPutImageDataHD

