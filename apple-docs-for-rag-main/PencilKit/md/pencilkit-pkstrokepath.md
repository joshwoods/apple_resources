

- PencilKit
-  PKStrokePath 

Structure

# PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct PKStrokePath
```

## Topics

### Creating a new stroke path

init()

Creates an empty stroke path.

init&lt;T>(controlPoints: T, creationDate: Date)

Creates a stroke path with the cubic B-spline control points and a date that you specify.

### Getting the stroke path properties

var creationDate: Date

The creation date and time of this stroke path.

### Accessing and interpolating points

func interpolatedPoints(in: ClosedRange&lt;CGFloat>?, by: PKStrokePath.InterpolatedSlice.Stride) -> PKStrokePath.InterpolatedSlice

Returns the slice on-curve points using the floating point range and stride that you specify.

func interpolatedLocation(at: CGFloat) -> CGPoint

Returns the on-curve point for the floating point parametric value.

func interpolatedPoint(at: CGFloat) -> PKStrokePoint

Returns the on-curve point for the provided floating point parameter.

func parametricValue(CGFloat, offsetBy: PKStrokePath.InterpolatedSlice.Stride) -> CGFloat

### Supporting types

struct InterpolatedSlice

A struct representing an interpolated slice of stroke points with a specific stride across a range of this stroke data.

### Supporting protocol requirements

Protocol implementations

Access the stroke path’s implementations of protocol methods.

### Using reference types

class PKStrokePathReference

A class that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- RandomAccessCollection
- Sequence

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

struct PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

struct PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

struct PKInk

A structure that represents an ink that specifies its type, color, and width.

