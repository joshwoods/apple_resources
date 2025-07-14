

- CarPlay
- CPMapTemplate
-  tripEstimateStyle 

Instance Property

# tripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var tripEstimateStyle: CPTripEstimateStyle { get set }
```

## Discussion

The default value is CPTripEstimateStyle.dark.

## See Also

### Providing Trip Estimates

func updateEstimates(CPTravelEstimates, for: CPTrip)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip.

func update(CPTravelEstimates, for: CPTrip, with: CPTimeRemainingColor)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip, with the specified time-remaining color.

enum CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

enum CPTripEstimateStyle

The set of display styles for trip estimates.

