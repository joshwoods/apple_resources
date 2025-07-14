

- Vision
-  NormalizedPoint 

Structure

# NormalizedPoint

A point in a 2D coordinate system.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct NormalizedPoint
```

## Topics

### Creating a normalized point

init(x: CGFloat, y: CGFloat)

Creates a point object with the specified coordinates.

init(normalizedPoint: CGPoint)

Creates a point object from the specified Core Graphics point.

init(imagePoint: CGPoint, in: CGSize)

Creates a normalized point from a point in an image coordinate space.

init(imagePoint: CGPoint, in: CGSize, normalizedTo: NormalizedRect)

Creates a point normalized to a region of interest within an image.

static var zero: NormalizedPoint

A point object that represents the origin.

### Inspecting a normalized point

let cgPoint: CGPoint

The Core Graphics point for this point.

var x: CGFloat

The x-coordinate.

var y: CGFloat

The y-coordinate.

### Converting points

func toImageCoordinates(from: NormalizedRect, imageSize: CGSize, origin: CoordinateOrigin) -> CGPoint

Converts a point normalized to a region within an image into full image coordinates.

func toImageCoordinates(CGSize, origin: CoordinateOrigin) -> CGPoint

Converts a point in normalized coordinates into image coordinates.

### Flipping a normalized point

func verticallyFlipped() -> NormalizedPoint

Returns a normalized point with the origin flipped between the top and bottom of the image.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Coordinate conversion

struct NormalizedRect

The location and dimensions of a rectangle.

struct NormalizedCircle

The center point and radius of a 2D circle.

enum CoordinateOrigin

The origin of a coordinate system relative to an image.

