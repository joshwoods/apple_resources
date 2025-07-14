

- SensorKit
- SRVisit
-  SRVisit.LocationCategory 

Enumeration

# SRVisit.LocationCategory

Types of locations.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum LocationCategory
```

## Topics

### Categories

case gym

The user’s gym.

case home

The user’s home.

case school

The user’s school.

case unknown

A location the user frequents that’s an unknown type.

case work

The user’s workplace.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Visit Information

var arrivalDateInterval: DateInterval

A range of time within which the user arrives at a location of interest.

var departureDateInterval: DateInterval

A range of time within which the user departs from a location of interest.

var distanceFromHome: CLLocationDistance

The location’s distance from the home-category location.

var locationCategory: SRVisit.LocationCategory

The location’s type.

