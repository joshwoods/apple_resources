

- UIKit
-  Drawing 

API Collection

# Drawing

Configure your app’s drawing environment using colors, renderers, draw paths, strings, and shadows.

## Topics

### UI updates

class UIUpdateLink

An object you use to observe, participate in, and affect the UI update process.

class UIUpdateInfo

An object that contains detailed information about the current UI update state.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

### Color

class UIColor

An object that stores color data and sometimes opacity.

### Graphics contexts

Use renderers to turn a set of programmatic drawing commands into a bitmap or PDF image.

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

### Paths

class UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

func UIRectFill(CGRect)

Fills the specified rectangle with the current color.

func UIRectFillUsingBlendMode(CGRect, CGBlendMode)

Fills a rectangle with the current fill color using the specified blend mode.

func UIRectFrame(CGRect)

Draws a frame around the inside of the specified rectangle.

func UIRectFrameUsingBlendMode(CGRect, CGBlendMode)

Draws a frame around the inside of a rectangle using the specified blend mode.

### Strings

class NSStringDrawingContext

An object that manages metrics for drawing attributed strings.

struct NSStringDrawingOptions

Constants that specify the rendering options for drawing a string.

enum UIBaselineAdjustment

Vertical adjustment options.

### Shadows

class NSShadow

An object you use to specify attributes to create and style a drop shadow during drawing operations.

### Graphics context primitives

Manage the current graphics environment using Core Graphics framework types.

func UIGraphicsGetCurrentContext() -> CGContext?

Returns the current graphics context.

func UIGraphicsPushContext(CGContext)

Makes the specified graphics context the current context.

func UIGraphicsPopContext()

Removes the current graphics context from the top of the stack, restoring the previous context.

func UIGraphicsBeginImageContextWithOptions(CGSize, Bool, CGFloat)

Creates a bitmap-based graphics context with the specified options.

Deprecated

func UIRectClip(CGRect)

Modifies the current clipping path by intersecting it with the specified rectangle.

### Primitive type conversions

class func cgAffineTransform(for: String) -> CGAffineTransform

Returns a Core Graphics affine transform structure corresponding to the data in a given string.

class func cgPoint(for: String) -> CGPoint

Returns a Core Graphics point structure corresponding to the data in a given string.

class func cgRect(for: String) -> CGRect

Returns a Core Graphics rectangle structure corresponding to the data in a given string.

class func cgSize(for: String) -> CGSize

Returns a Core Graphics size structure corresponding to the data in a given string.

class func cgVector(for: String) -> CGVector

Returns a Core Graphics vector corresponding to the data in a given string.

class func string(for: CGAffineTransform) -> String

Returns a string formatted to contain the data from an affine transform.

class func string(for: CGPoint) -> String

Returns a string formatted to contain the data from a point.

class func string(for: CGRect) -> String

Returns a string formatted to contain the data from a rectangle.

class func string(for: CGSize) -> String

Returns a string formatted to contain the data from a size data structure.

class func string(for: CGVector) -> String

Returns a string formatted to contain the data from a vector data structure.

## See Also

### Graphics, drawing, and printing

Images and PDF

Create and manage images, including those that use bitmap and PDF formats.

Printing

Display the system print panels and manage the printing process.

