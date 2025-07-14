

- PencilKit
-  PKStrokePoint 

Structure

# PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct PKStrokePoint
```

## Topics

### Creating a stroke point object

init(location: CGPoint, timeOffset: TimeInterval, size: CGSize, opacity: CGFloat, force: CGFloat, azimuth: CGFloat, altitude: CGFloat)

Creates a new point with the provided properties.

init(location: CGPoint, timeOffset: TimeInterval, size: CGSize, opacity: CGFloat, force: CGFloat, azimuth: CGFloat, altitude: CGFloat, secondaryScale: CGFloat)

### Getting the point’s location

var location: CGPoint

The location of this point.

var timeOffset: TimeInterval

The time offset since the start of the stroke path in seconds.

### Getting the point’s touch data

var altitude: CGFloat

The altitude of this point in radians.

var azimuth: CGFloat

The azimuth of this point in radians.

var force: CGFloat

The amount of force applied by the touch.

### Getting the point’s drawing data

var size: CGSize

The size of this point.

var opacity: CGFloat

Opacity of the point.

var secondaryScale: CGFloat

### Using reference types

class PKStrokePointReference

A class that represents the properties of a specific point along a stroke’s path.

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

struct PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

struct PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

struct PKInk

A structure that represents an ink that specifies its type, color, and width.

