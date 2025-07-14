

- CarPlay
-  CPLaneStatus 

Enumeration

# CPLaneStatus

Values that describe the status or preferability of a lane.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
enum CPLaneStatus
```

## Topics

### Initializers

init?(rawValue: Int)

Creates a lane status with the provided value.

### Lane statuses

case notGood

The lane status is not good.

case good

The lane status is good.

case preferred

The lane status is preferred.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Routes, lanes and junctions

class CPRouteInformation

A class that describes the characteristic elements of a route.

class CPLane

A class that describes characteristics of a lane on a roadway.

class CPLaneGuidance

A class that provides information that describes the number of lanes on a roadway and navigation instruction variants.

enum CPJunctionType

Values that represent types of roadway junctions.

