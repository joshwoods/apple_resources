

- PencilKit
-  PKStroke 

Structure

# PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct PKStroke
```

## Mentioned in 

Supporting backward compatibility for ink types

## Topics

### Creating a stroke object

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: NSBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?, randomSeed: UInt32)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: NSBezierPath?, randomSeed: UInt32)

Creates a macOS stroke with the line properties, path, transform, mask, and random seed that you specify.

### Getting the stroke properties

var ink: PKInk

The Ink, which is a combination of a tool used to render this stroke.

var mask: UIBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var mask: NSBezierPath?

The pretransform mask used to clip the rendering of the stroke.

var maskedPathRanges: [ClosedRange&lt;CGFloat>]

The range of points in the stroke path reference that intersect the stroke’s mask.

var path: PKStrokePath

The B-spline path that describes this stroke.

var renderBounds: CGRect

The bounds of the rendered stroke, including the width and line properties of the stroke after applying the transform.

var transform: CGAffineTransform

The affine transform of the stroke after rendering.

var randomSeed: UInt32

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the stroke.

### Using reference types

class PKStrokeReference

A class that represents the paths, boundaries and other properties of a stroke drawn on a canvas.

## Relationships

### Conforms To

- Copyable

## See Also

### Canvas

Drawing with PencilKit

Add expressive, low-latency drawing to your app using PencilKit.

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

Inspecting, Modifying, and Constructing PencilKit Drawings

Score users’ ability to match PencilKit drawings generated from text, by accessing the strokes and points inside PencilKit drawings.

class PKCanvasView

A view that captures Apple Pencil input and displays the rendered results in an iOS app.

struct PKDrawing

A structure representing the drawing information captured by a canvas view.

struct PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

struct PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

struct PKInk

A structure that represents an ink that specifies its type, color, and width.

