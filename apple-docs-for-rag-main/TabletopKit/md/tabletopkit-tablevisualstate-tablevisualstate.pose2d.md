

- TabletopKit
- TableVisualState
-  TableVisualState.Pose2D 

Structure

# TableVisualState.Pose2D

An object that represents a 2D position and orientation on the XZ plane.

visionOS 2.0+

``` source
struct Pose2D
```

## Topics

### Creating 2D pose objects

init()

init(position: TableVisualState.Point2D, rotation: Angle2D)

### Getting 2D pose properties

var position: TableVisualState.Point2D

var rotation: Angle2D

### Getting the identifier

static var identity: TableVisualState.Pose2D

The identity pose

### Initializers

init(projecting: Pose3D)

Initializes this pose as the 2D projection of the given pose on the XZ plane

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

struct Point2D

An object that represents a point on the XZ plane.

