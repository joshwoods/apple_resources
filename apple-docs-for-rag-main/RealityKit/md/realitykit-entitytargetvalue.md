

- RealityKit
-  EntityTargetValue 

Structure

# EntityTargetValue

A value containing an original gesture value along with a targeted entity.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@dynamicMemberLookup
struct EntityTargetValue
```

## Overview

Spatial data from a location returned by a gesture can be converted to and from the entity using functions defined in RealityCoordinateSpaceConverting.

For example, here’s how to convert location from a DragGesture to the parent of an Entity:

```
DragGesture(coordinateSpace: .global).targetedToEntity().updating($state) { state, value, _ in
    let location = value.convert(
        value.location, from: .global, to: value.entity.parent
    )
    ...
}
```

## Topics

### Accessing gesture info

var entity: Entity

The targeted entity.

var gestureValue: Value

The gesture value updated by the gesture.

subscript&lt;T>(dynamicMember _: KeyPath&lt;Value, T>) -> T

### Instance Methods

func unproject(CGPoint, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> SIMD3&lt;Float>?

Unproject `point` from a 2D coordinate space into 3D world coordinates.

func unproject(KeyPath&lt;Value, CGPoint>, to: some RealityCoordinateSpace) -> SIMD3&lt;Float>?

Unproject a 2D point from the gesture value into 3D world coordinates.

### Default Implementations

Equatable Implementations

RealityCoordinateSpaceConverting Implementations

RealityCoordinateSpaceProjecting Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- RealityCoordinateSpaceConverting

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

- RealityCoordinateSpaceProjecting

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

## See Also

### Direct and indirect gestures

Transforming RealityKit entities using gestures

Build a RealityKit component to support standard visionOS gestures on any entity.

struct InputTargetComponent

A component that gives an entity the ability to receive system input.

