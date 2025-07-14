

- CarPlay
-  CPManeuverType 

Enumeration

# CPManeuverType

Values that describe types of navigation maneuvers.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
enum CPManeuverType
```

## Topics

### Initializers

init?(rawValue: UInt)

Creates a new maneuver type with the provided value.

### Maneuver types

case arriveAtDestination

case arriveAtDestinationLeft

case arriveAtDestinationRight

case arriveEndOfDirections

case arriveEndOfNavigation

case changeFerry

case changeHighway

case changeHighwayLeft

case changeHighwayRight

case enterRoundabout

case enter_Ferry

case exitFerry

case exitRoundabout

case followRoad

case highwayOffRampLeft

case highwayOffRampRight

case keepLeft

case keepRight

case leftTurn

case leftTurnAtEnd

case noTurn

case offRamp

case onRamp

case rightTurn

case rightTurnAtEnd

case roundaboutExit1

case roundaboutExit10

case roundaboutExit11

case roundaboutExit12

case roundaboutExit13

case roundaboutExit14

case roundaboutExit15

case roundaboutExit16

case roundaboutExit17

case roundaboutExit18

case roundaboutExit19

case roundaboutExit2

case roundaboutExit3

case roundaboutExit4

case roundaboutExit5

case roundaboutExit6

case roundaboutExit7

case roundaboutExit8

case roundaboutExit9

case sharpLeftTurn

case sharpRightTurn

case slightLeftTurn

case slightRightTurn

case startRoute

case startRouteWithUTurn

case straightAhead

case uTurn

case uTurnAtRoundabout

case uTurnWhenPossible

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Maneuvers

class CPManeuver

An object that describes a single navigation instruction.

enum CPManeuverState

Values that describe the state of a maneuver.

