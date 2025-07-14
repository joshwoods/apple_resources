

- TabletopKit
- TableVisualState
-  TableVisualState.Point2D 

Structure

# TableVisualState.Point2D

An object that represents a point on the XZ plane.

visionOS 2.0+

``` source
struct Point2D
```

## Topics

### Creating 2D point states

init()

init(projecting: Point3D)

Initializes this point as the projection of the given 3D point on the XZ plane

init(x: Double, z: Double)

### Getting 2D point properties

var x: Double

var z: Double

static let zero: TableVisualState.Point2D

### Default Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Representing 2D states

struct Pose2D

An object that represents a 2D position and orientation on the XZ plane.

