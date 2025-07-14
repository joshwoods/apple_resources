

- SwiftUI
-  PhysicalMetric 

Structure

# PhysicalMetric

Provides access to a value in points that corresponds to the specified physical measurement.

visionOS 1.0+

``` source
@propertyWrapper @frozen
struct PhysicalMetric
```

## Overview

Use this property wrapper inside a View or a type that inherits a `View`’s environment, like a ViewModifier. Its value will be the equivalent in points of the physical measurement of length you specify.

For example, to have a variable that contains the amount of points corresponding to one meter, you can do the following:

```
struct MyView: View {
    @PhysicalMetric(from: .meters)
    var twoAndAHalfMeters = 2.5
    …
}
```

Using this wrapper for a property of a type not associated with a scene’s view contents, like an App or a Scene, is unsupported.

## Compensating for World Scaling

Starting with apps built against the visionOS 2.0 SDK, the default behavior of `PhysicalMetric` is to produce values that match the distances used by `RealityView`s in the same scene, by scaling its returned values to match the world scaling of the current scene. Previously, the values were not scaled, and they were suitable for measuring distances and lengths within the user’s surroundings, outside of any scene. Unscaled values could produce unexpected behavior if used in conjunction with `RealityView`s within the scene.

To modify the behavior of `PhysicalMetric` and obtain unscaled values, use the transformEnvironment(_:transform:) modifier, transforming the physicalMetrics key path, to edit the converter used by `PhysicalMetric` within the modified views to use a new WorldScalingCompensation mode. For example:

```
struct RulerView: View {
    @PhysicalMetric(from: .meters)
    var oneMeter = 1

    var body: some View {
        /* implement a size-accurate ruler */
    }
}

struct ContentView: View {
    var body: some View {
        RulerView()
            .transformEnvironment(\.physicalMetrics) { metrics in
                metrics = metrics.worldScalingCompensation(.unscaled)
            }
    }
}
```

See Also

PhysicalMetricsConverter

See Also

WorldScalingCompensation

## Topics

### Creating a metric

init(wrappedValue:from:)

Creates a value that maps the specified point, whose dimensions are specified in physical length measurements in the given unit, to the corresponding value in points in the associated scene.

### Getting the value

var wrappedValue: Value

A value in points in the coordinate system of the associated scene.

## Relationships

### Conforms To

- DynamicProperty

## See Also

### Measuring a view

struct GeometryReader

A container view that defines its content as a function of its own size and coordinate space.

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

struct PhysicalMetricsConverter

A physical metrics converter provides conversion between point values and their extent in 3D space, in the form of physical length measurements.

