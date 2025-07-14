

- CarPlay
-  CPJunctionType 

Enumeration

# CPJunctionType

Values that represent types of roadway junctions.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
enum CPJunctionType
```

## Topics

### Initializers

init?(rawValue: UInt)

Creates a junction type with the provided integer value.

### Junction types

case intersection

A single intersection with roads coming to a common point.

case roundabout

Junction elements that represent roads exiting the roundabout.

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

enum CPLaneStatus

Values that describe the status or preferability of a lane.

