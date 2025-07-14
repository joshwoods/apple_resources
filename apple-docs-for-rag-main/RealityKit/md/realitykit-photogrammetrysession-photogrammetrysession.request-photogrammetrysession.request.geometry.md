

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.Geometry 

Structure

# PhotogrammetrySession.Request.Geometry

An object that holds a bounding box and transformation data for a request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Geometry
```

## Topics

### Creating a geometry instance

init(bounds: BoundingBox, transform: Transform)

Creates an instance with an optional bounding box and transform.

### Accessing geometry data

var bounds: BoundingBox

The bounding box for the created entity.

var transform: Transform

A transform applied to the created entity.

### Comparing geometry values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (PhotogrammetrySession.Request.Geometry, PhotogrammetrySession.Request.Geometry) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(orientedBounds: OrientedBoundingBox, transform: Transform)

Creates an instance from an oriented bounding box and transform.

### Instance Properties

var orientedBounds: OrientedBoundingBox

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

