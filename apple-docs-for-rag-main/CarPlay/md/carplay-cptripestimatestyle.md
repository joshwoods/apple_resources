

- CarPlay
-  CPTripEstimateStyle 

Enumeration

# CPTripEstimateStyle

The set of display styles for trip estimates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
enum CPTripEstimateStyle
```

## Topics

### Styles

case light

The light trip estimate display style.

case dark

The dark trip estimate display style.

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

enum CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

var tripEstimateStyle: CPTripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

