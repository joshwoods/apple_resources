

- CarPlay
- CPMapTemplate
-  update(\_:for:with:) 

Instance Method

# update(\_:for:with:)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip, with the specified time-remaining color.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func update(
    _ estimates: CPTravelEstimates,
    for trip: CPTrip,
    with timeRemainingColor: CPTimeRemainingColor
)
```

## Parameters 

`estimates`  

The updated travel estimates.

`trip`  

A trip preview or the active trip.

`timeRemainingColor`  

The time-remaining color.

## See Also

### Providing Trip Estimates

func updateEstimates(CPTravelEstimates, for: CPTrip)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip.

enum CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

var tripEstimateStyle: CPTripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

enum CPTripEstimateStyle

The set of display styles for trip estimates.

