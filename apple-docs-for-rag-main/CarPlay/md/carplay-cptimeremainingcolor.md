

- CarPlay
-  CPTimeRemainingColor 

Enumeration

# CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum CPTimeRemainingColor
```

## Overview

The system determines the shade of each color based on the tripEstimateStyle for the map template.

## Topics

### Colors

case `default`

The system default color.

case green

A shade of green.

case orange

A shade of orange.

case red

A shade of red.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing Trip Estimates

func updateEstimates(CPTravelEstimates, for: CPTrip)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip.

func update(CPTravelEstimates, for: CPTrip, with: CPTimeRemainingColor)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip, with the specified time-remaining color.

var tripEstimateStyle: CPTripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

enum CPTripEstimateStyle

The set of display styles for trip estimates.

