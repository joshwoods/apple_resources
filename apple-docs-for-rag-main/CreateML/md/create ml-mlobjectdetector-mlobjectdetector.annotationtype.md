

- Create ML
- MLObjectDetector
-  MLObjectDetector.AnnotationType 

Enumeration

# MLObjectDetector.AnnotationType

The available types of image annotations.

macOS 10.15+

``` source
enum AnnotationType
```

## Mentioned in 

Building an object detector data source

## Overview

Use MLObjectDetector.AnnotationType to tell Create ML how to interpret your object annotations.

## Topics

### Bounding box annotations

case boundingBox(units: MLBoundingBoxUnits, origin: MLBoundingBoxCoordinatesOrigin, anchor: MLBoundingBoxAnchor)

An annotation type that defines a rectangle around an object within an image.

enum MLBoundingBoxUnits

The units a bounding box annotation uses to define its position and size.

enum MLBoundingBoxAnchor

A location within a bounding box that an annotation’s coordinates use as their reference point.

enum MLBoundingBoxCoordinatesOrigin

The location within an image that an annotation’s coordinates use as their origin.

## Relationships

### Conforms To

- Sendable

## See Also

### Supporting types

enum DataSource

A data source for an object detector.

struct ModelParameters

Parameters that affect the process of training an object detection model.

