

- AppKit
-  NSGradient 

Class

# NSGradient

An object that can draw gradient fill colors

macOS 10.5+

``` source
class NSGradient
```

## Overview

This class provides convenience methods for drawing radial or linear (axial) gradients for rectangles and NSBezierPath objects. It also supports primitive methods that let you customize the shape of the gradient fill. A gradient consists of two or more color changes over the range of the gradient shape. When creating a gradient object, you specify the colors and their locations relative to the start and end of the gradient. This combination of color and location is known as a *color stop*. During drawing, the NSGradient object uses the color stop information to compute color changes for you and passes that information to the Quartz shading functions.

Because the NSGradient class uses Quartz shadings, drawing is handled by computing the colors at a given point mathematically. This technique results in smooth gradients regardless of the resolution of the target device.

For more information about gradients and their appearance, see Gradients in Quartz 2D Programming Guide.

## Topics

### Creating a Gradient

convenience init?(starting: NSColor, ending: NSColor)

Initializes a newly allocated gradient object with two colors.

convenience init?(colors: [NSColor])

Initializes a newly allocated gradient object with an array of colors.

convenience init?(colorsAndLocations: (NSColor, CGFloat)...)

Initializes a newly allocated gradient object with a comma-separated list of arguments.

init?(colors: [NSColor], atLocations: UnsafePointer&lt;CGFloat>?, colorSpace: NSColorSpace)

Initializes a newly allocated gradient object with the specified colors, color locations, and color space.

init?(coder: NSCoder)

Creates a gradient from data in an unarchiver.

### Drawing a Linear Gradient

func draw(from: NSPoint, to: NSPoint, options: NSGradient.DrawingOptions)

Draws a linear gradient between the specified start and end points.

func draw(in: NSRect, angle: CGFloat)

Fills the specified rectangle with a linear gradient.

func draw(in: NSBezierPath, angle: CGFloat)

Fills the specified path with a linear gradient.

### Drawing a Radial Gradient

func draw(fromCenter: NSPoint, radius: CGFloat, toCenter: NSPoint, radius: CGFloat, options: NSGradient.DrawingOptions)

Draws a radial gradient between the specified circles.

func draw(in: NSRect, relativeCenterPosition: NSPoint)

Draws a radial gradient starting at the center of the specified rectangle.

func draw(in: NSBezierPath, relativeCenterPosition: NSPoint)

Draws a radial gradient starting at the center point of the specified path.

### Getting Gradient Properties

var colorSpace: NSColorSpace

The color space of the colors associated with the gradient.

var numberOfColorStops: Int

The number of color stops associated with the gradient.

func getColor(AutoreleasingUnsafeMutablePointer&lt;NSColor>?, location: UnsafeMutablePointer&lt;CGFloat>?, at: Int)

Returns information about the color stop at the specified index in the receiver’s color array.

func interpolatedColor(atLocation: CGFloat) -> NSColor

Returns the color of the rendered gradient at the specified relative location.

### Constants

struct DrawingOptions

Constants that specify gradient drawing options.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

