

- CarPlay
-  CPLaneGuidance 

Class

# CPLaneGuidance

A class that provides information that describes the number of lanes on a roadway and navigation instruction variants.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
class CPLaneGuidance
```

## Topics

### Properties

var instructionVariants: [String]

An array of strings that represent the instruction for this lane guidance, arranged from most- to least-preferred.

var lanes: [CPLane]

An array of lane objects, each describing a single lane.

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

class CPLane

A class that describes characteristics of a lane on a roadway.

enum CPLaneStatus

Values that describe the status or preferability of a lane.

enum CPJunctionType

Values that represent types of roadway junctions.

