

- CarPlay
-  CPLane 

Class

# CPLane

A class that describes characteristics of a lane on a roadway.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class CPLane
```

## Topics

### Properties

var primaryAngle: Measurement&lt;UnitAngle>

A value that represents the angle the framework highlights if this lane is preferred or good.

Deprecated

var secondaryAngles: [Measurement&lt;UnitAngle>]

A list of the remaining angles of this lane guidance.

Deprecated

var status: CPLaneStatus

A value that describes the lane’s status.

### Lane status

enum CPLaneStatus

Values that describe the status or preferability of a lane.

### Initializers

init()Deprecated

init(angles: [Measurement&lt;UnitAngle>])

init(angles: [Measurement&lt;UnitAngle>], highlightedAngle: Measurement&lt;UnitAngle>, isPreferred: Bool)

### Instance Properties

var angles: [Measurement&lt;UnitAngle>]

var highlightedAngle: Measurement&lt;UnitAngle>?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Routes, lanes and junctions

class CPRouteInformation

A class that describes the characteristic elements of a route.

class CPLaneGuidance

A class that provides information that describes the number of lanes on a roadway and navigation instruction variants.

enum CPLaneStatus

Values that describe the status or preferability of a lane.

enum CPJunctionType

Values that represent types of roadway junctions.

