

- ARKit
- ARPlaneAnchor
-  ARPlaneAnchor.Classification 

Enumeration

# ARPlaneAnchor.Classification

Possible characterizations of real-world surfaces represented by plane anchors.

iOS 12.0+iPadOS 12.0+

``` source
enum Classification
```

## Overview

You get values of this type from a plane anchor’s classification property, identifying both the likely type of real-world surface for a detected plane anchor and the state of ARKit’s plane classification process.

## Topics

### Plane Classifications

case wall

The plane anchor represents a real-world wall or similar large vertical surface.

case floor

The plane anchor represents a real-world floor, ground plane, or similar large horizontal surface.

case ceiling

The plane anchor represents a real-world ceiling or similar overhead horizontal surface.

case table

The plane anchor represents a real-world table, desk, bar, or similar flat surface.

case seat

The plane anchor represents a real-world chair, stool, bench or similar flat surface.

case door

The plane anchor represents a real-world door or similar vertical surface.

case window

The plane anchor represents a real-world window or similar vertical surface.

### Missing Classification Status

case none(ARPlaneAnchor.Classification.Status)

No classification is available for the plane anchor.

enum Status

Reasons ARKit is unable to classify a plane.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Classifying a Plane

class var isClassificationSupported: Bool

A Boolean value that indicates whether plane classification is available on the current device.

var classification: ARPlaneAnchor.Classification

A general characterization of what kind of real-world surface the plane anchor represents.

