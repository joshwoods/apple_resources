

- MapKit
-  MKOverlayPathRenderer 

Class

# MKOverlayPathRenderer

The visual representation of a path-based overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKOverlayPathRenderer
```

## Overview

Use this renderer when a CGPath object defines your overlay’s shape. By default, this renderer fills the overlay’s shape and represents the strokes of the path using its current attributes.

You can use this class as-is or subclass it to define additional drawing behaviors. If you subclass it, override the createPath() method and use that method to build the appropriate path object. To change the path, invalidate it and recreate the path using the new data your subclass obtains.

## Topics

### Creating and managing the path

var path: CGPath!

The path representing the overlay’s shape.

func createPath()

Creates the path for the overlay.

func invalidatePath()

Updates the path associated with the overlay renderer.

### Accessing the drawing attributes

var fillColor: UIColor?

The fill color to use for the path.

var strokeColor: UIColor?

The stroke color to use for the path.

var lineWidth: CGFloat

The stroke width to use for the path.

var lineJoin: CGLineJoin

The line join style to apply to the corners of the path.

var lineCap: CGLineCap

The line cap style to apply to the open ends of the path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var lineDashPhase: CGFloat

The offset (in points) at which to start drawing the dash pattern.

var lineDashPattern: [NSNumber]?

An array of numbers specifying the dash pattern to use for the path.

### Drawing the path

func applyStrokeProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the renderer’s stroke-related drawing properties to the specified graphics context.

func applyFillProperties(to: CGContext, atZoomScale: MKZoomScale)

Applies the receiver’s fill-related drawing properties to the specified graphics context.

func strokePath(CGPath, in: CGContext)

Draws a line along the specified path.

func fillPath(CGPath, in: CGContext)

Fills the area that the specified path encloses.

var shouldRasterize: Bool

A Boolean value that determines whether the overlay path renderer renders the overlay as a bitmap before compositing.

## Relationships

### Inherits From

- MKOverlayRenderer

### Inherited By

- MKCircleRenderer
- MKMultiPolygonRenderer
- MKMultiPolylineRenderer
- MKPolygonRenderer
- MKPolylineRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Custom shape overlays

class MKPolygon

A closed polygon overlay.

class MKPolygonRenderer

The visual representation of a single polygon overlay.

class MKMultiPolygon

A collection of multiple closed polygon overlays.

class MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

