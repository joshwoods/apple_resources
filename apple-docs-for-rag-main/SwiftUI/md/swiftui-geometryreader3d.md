

- SwiftUI
-  GeometryReader3D 

Structure

# GeometryReader3D

A container view that defines its content as a function of its own size and coordinate space.

visionOS 1.0+

``` source
@frozen
struct GeometryReader3D where Content : View
```

## Overview

This view returns a flexible preferred size to its own container view.

This container differs from GeometryReader in that it also reads available depth, and thus also returns a flexible preferred depth to its parent layout. Use the 3D version only in situations where you need to read depth, because it affects depth layout when used in a container like a ZStack.

## Topics

### Creating a geometry reader

init(content: (GeometryProxy3D) -> Content)

var content: (GeometryProxy3D) -> Content

## Relationships

### Conforms To

- View

## See Also

### Measuring a view

struct GeometryReader

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

