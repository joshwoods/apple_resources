

- SwiftUI
-  GeometryReader 

Structure

# GeometryReader

A container view that defines its content as a function of its own size and coordinate space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct GeometryReader where Content : View
```

## Overview

This view returns a flexible preferred size to its parent layout.

## Topics

### Creating a geometry reader

init(content: (GeometryProxy) -> Content)

var content: (GeometryProxy) -> Content

## Relationships

### Conforms To

- View

## See Also

### Measuring a view

struct GeometryReader3D

A container view that defines its content as a function of its own size and coordinate space.

struct GeometryProxy

A proxy for access to the size and coordinate space (for anchor resolution) of the container view.

struct GeometryProxy3D

A proxy for access to the size and coordinate space of the container view.

func coordinateSpace(NamedCoordinateSpace) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

enum CoordinateSpace

A resolved coordinate space created by the coordinate space protocol.

protocol CoordinateSpaceProtocol

A frame of reference within the layout system.

struct PhysicalMetric

Provides access to a value in points that corresponds to the specified physical measurement.

struct PhysicalMetricsConverter

A physical metrics converter provides conversion between point values and their extent in 3D space, in the form of physical length measurements.

