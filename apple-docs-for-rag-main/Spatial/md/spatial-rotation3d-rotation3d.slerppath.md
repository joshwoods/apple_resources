

- Spatial
- Rotation3D
-  Rotation3D.SlerpPath 

Enumeration

# Rotation3D.SlerpPath

Constants that define the arc that a slerp operation takes.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum SlerpPath
```

## Topics

### Enumeration Cases

case automatic

Spherical linear interpolation along the automatically selected arc between two rotations.

case shortest

Spherical linear interpolation along the shortest arc between two rotations.

case longest

Spherical linear interpolation along the longest arc between two rotations.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Operator Functions

static func == (Rotation3D, Rotation3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Transforming a 3D rotation structure

static func slerp(from: Rotation3D, to: Rotation3D, t: Double, along: Rotation3D.SlerpPath) -> Rotation3D

Returns the spherical linear interpolation along either the shortest or the longest arc between two rotations.

var inverse: Rotation3D

The inverse of the rotation.

static let identity: Rotation3D

The identity rotation.

