

- Create ML
-  MLBoundingBoxCoordinatesOrigin 

Enumeration

# MLBoundingBoxCoordinatesOrigin

The location within an image that an annotation’s coordinates use as their origin.

macOS 10.15+

``` source
enum MLBoundingBoxCoordinatesOrigin
```

## Topics

### Designating origins

case topLeft

An origin at the image’s top-left corner.

case bottomLeft

An origin at the image’s bottom-left corner.

### Comparing errors

static func == (MLBoundingBoxCoordinatesOrigin, MLBoundingBoxCoordinatesOrigin) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Getting the hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Bounding box annotations

case boundingBox(units: MLBoundingBoxUnits, origin: MLBoundingBoxCoordinatesOrigin, anchor: MLBoundingBoxAnchor)

An annotation type that defines a rectangle around an object within an image.

enum MLBoundingBoxUnits

The units a bounding box annotation uses to define its position and size.

enum MLBoundingBoxAnchor

A location within a bounding box that an annotation’s coordinates use as their reference point.

