

- SwiftUI
-  GeometryProxy3D 

Structure

# GeometryProxy3D

A proxy for access to the size and coordinate space of the container view.

visionOS 1.0+

``` source
struct GeometryProxy3D
```

## Overview

You can use a proxy for anchor resolution.

## Topics

### Accessing geometry characteristics

func frame(in: some CoordinateSpaceProtocol) -> Rect3D

The container view’s bounds rectangle converted to a defined coordinate space.

var size: Size3D

The size of the container view.

var safeAreaInsets: EdgeInsets3D

The safe area inset of the container view.

subscript&lt;T>(Anchor&lt;T>) -> T

Resolves the value of an anchor to the container view.

func transform(in: some CoordinateSpaceProtocol) -> AffineTransform3D?

The container view’s 3D transform converted to a defined coordinate space.

## See Also

### Measuring a view

struct GeometryReader

A container view that defines its content as a function of its own size and coordinate space.

struct GeometryReader3D

A container view that defines its content as a function of its own size and coordinate space.

struct GeometryProxy

A proxy for access to the size and coordinate space (for anchor resolution) of the container view.

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

