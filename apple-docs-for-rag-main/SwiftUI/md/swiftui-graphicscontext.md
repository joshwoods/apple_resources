

- SwiftUI
-  GraphicsContext 

Structure

# GraphicsContext

An immediate mode drawing destination, and its current state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct GraphicsContext
```

## Overview

Use a context to execute 2D drawing primitives. For example, you can draw filled shapes using the fill(_:with:style:) method inside a Canvas view:

```
Canvas { context, size in
    context.fill(
        Path(ellipseIn: CGRect(origin: .zero, size: size)),
        with: .color(.green))
}
.frame(width: 300, height: 200)
```

The example above draws an ellipse that just fits inside a canvas that’s constrained to 300 points wide and 200 points tall:

In addition to outlining or filling paths, you can draw images, text, and SwiftUI views. You can also use the context to perform many common graphical operations, like adding masks, applying filters and transforms, and setting a blend mode. For example you can add a mask using the clip(to:style:options:) method:

```
let halfSize = size.applying(CGAffineTransform(scaleX: 0.5, y: 0.5))
context.clip(to: Path(CGRect(origin: .zero, size: halfSize)))
context.fill(
    Path(ellipseIn: CGRect(origin: .zero, size: size)),
    with: .color(.green))
```

The rectangular mask hides all but one quadrant of the ellipse:

The order of operations matters. Changes that you make to the state of the context, like adding a mask or a filter, apply to later drawing operations. If you reverse the fill and clip operations in the example above, so that the fill comes first, the mask doesn’t affect the ellipse.

Each context references a particular layer in a tree of transparency layers, and also contains a full copy of the drawing state. You can modify the state of one context without affecting the state of any other, even if they refer to the same layer. For example you can draw the masked ellipse from the previous example into a copy of the main context, and then add a rectangle into the main context:

```
// Create a copy of the context to draw a clipped ellipse.
var maskedContext = context
let halfSize = size.applying(CGAffineTransform(scaleX: 0.5, y: 0.5))
maskedContext.clip(to: Path(CGRect(origin: .zero, size: halfSize)))
maskedContext.fill(
    Path(ellipseIn: CGRect(origin: .zero, size: size)),
    with: .color(.green))

// Go back to the original context to draw the rectangle.
let origin = CGPoint(x: size.width / 4, y: size.height / 4)
context.fill(
    Path(CGRect(origin: origin, size: halfSize)),
    with: .color(.blue))
```

The mask doesn’t clip the rectangle because the mask isn’t part of the main context. However, both contexts draw into the same view because you created one context as a copy of the other:

The context has access to an EnvironmentValues instance called environment that’s initially copied from the environment of its enclosing view. SwiftUI uses environment values — like the display resolution and color scheme — to resolve types like Image and Color that appear in the context. You can also access values stored in the environment for your own purposes.

## Topics

### Drawing a path

func stroke(Path, with: GraphicsContext.Shading, lineWidth: CGFloat)

Draws a path into the context with a specified line width.

func stroke(Path, with: GraphicsContext.Shading, style: StrokeStyle)

Draws a path into the context with a specified stroke style.

func fill(Path, with: GraphicsContext.Shading, style: FillStyle)

Draws a path into the context and fills the outlined region.

struct Shading

A color or pattern that you can use to outline or fill a path.

struct GradientOptions

Options that affect the rendering of color gradients.

### Drawing images, text, and views

func draw(_:in:)

Draws a resolved symbol into the context, using the specified rectangle as a layout frame.

func draw(_:in:style:)

Draws a resolved image into the context, using the specified rectangle as a layout frame.

func draw(_:at:anchor:)

Draws a resolved image into the context, aligning an anchor within the image to a point in the context.

### Drawing into a new layer

func drawLayer(content: (inout GraphicsContext) throws -> Void) rethrows

Draws a new layer, created by drawing code that you provide, into the context.

### Resolving a drawn entity

func resolve(_:)

Gets a version of an image that’s fixed with the current values of the graphics context’s environment.

func resolveSymbol&lt;ID>(id: ID) -> GraphicsContext.ResolvedSymbol?

Gets the identified child view as a resolved symbol, if the view exists.

struct ResolvedSymbol

A static sequence of drawing operations that may be drawn multiple times, preserving their resolution independence.

struct ResolvedImage

An image resolved to a particular environment.

struct ResolvedText

A text view resolved to a particular environment.

### Masking

func clip(to: Path, style: FillStyle, options: GraphicsContext.ClipOptions)

Adds a path to the context’s array of clip shapes.

func clipToLayer(opacity: Double, options: GraphicsContext.ClipOptions, content: (inout GraphicsContext) throws -> Void) rethrows

Adds a clip shape that you define in a new layer to the context’s array of clip shapes.

var clipBoundingRect: CGRect

The bounding rectangle of the intersection of all current clip shapes in the current user space.

struct ClipOptions

Options that affect the use of clip shapes.

### Setting opacity and the blend mode

var opacity: Double

The opacity of drawing operations in the context.

var blendMode: GraphicsContext.BlendMode

The blend mode used by drawing operations in the context.

struct BlendMode

The ways that a graphics context combines new content with background content.

### Filtering

func addFilter(GraphicsContext.Filter, options: GraphicsContext.FilterOptions)

Adds a filter that applies to subsequent drawing operations.

struct Filter

A type that applies image processing operations to rendered content.

struct FilterOptions

Options that configure a filter that you add to a graphics context.

struct BlurOptions

Options that configure the graphics context filter that creates blur.

struct ShadowOptions

Options that configure the graphics context filter that creates shadows.

### Applying transforms

func scaleBy(x: CGFloat, y: CGFloat)

Scales subsequent drawing operations by an amount in each dimension.

func rotate(by: Angle)

Rotates subsequent drawing operations by an angle.

func translateBy(x: CGFloat, y: CGFloat)

Moves subsequent drawing operations by an amount in each dimension.

func concatenate(CGAffineTransform)

Appends the given transform to the context’s existing transform.

var transform: CGAffineTransform

The current transform matrix, defining user space coordinates.

### Drawing with a core graphics context

func withCGContext(content: (CGContext) throws -> Void) rethrows

Provides a Core Graphics context that you can use as a proxy to draw into this context.

### Accessing the environment

var environment: EnvironmentValues

The environment associated with the graphics context.

### Instance Methods

func draw(_:options:)

Draws `line` into the graphics context.

## See Also

### Immediate mode drawing

Add Rich Graphics to Your SwiftUI App

Make your apps stand out by adding background materials, vibrancy, custom graphics, and animations.

struct Canvas

A view type that supports immediate mode drawing.

