

- Create ML
-  MLBoundingBoxUnits 

Enumeration

# MLBoundingBoxUnits

The units a bounding box annotation uses to define its position and size.

macOS 10.15+

``` source
enum MLBoundingBoxUnits
```

## Overview

All bounding box annotations in an annotation file must use the same units for their coordinates and size. See MLObjectDetector.AnnotationType.boundingBox(units:origin:anchor:).

## Topics

### Designating units

case pixel

A unit of measurement in pixels for an image.

case normalized

A unit of measurement as a portion of an image’s overall width or height.

### Comparing errors

static func == (MLBoundingBoxUnits, MLBoundingBoxUnits) -> Bool

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

enum MLBoundingBoxAnchor

A location within a bounding box that an annotation’s coordinates use as their reference point.

enum MLBoundingBoxCoordinatesOrigin

The location within an image that an annotation’s coordinates use as their origin.

