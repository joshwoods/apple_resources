

- CarPlay
- CPMapTemplate
-  updateEstimates(\_:for:) 

Instance Method

# updateEstimates(\_:for:)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func updateEstimates(
    _ estimates: CPTravelEstimates,
    for trip: CPTrip
)
```

## Parameters 

`estimates`  

The updated travel estimates.

`trip`  

A trip preview or the active trip.

## Discussion

The updated trip uses the default time-remaining color. To change the color, use the update(_:for:with:) method instead of calling this method.

## See Also

### Providing Trip Estimates

func update(CPTravelEstimates, for: CPTrip, with: CPTimeRemainingColor)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip, with the specified time-remaining color.

enum CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

var tripEstimateStyle: CPTripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

enum CPTripEstimateStyle

The set of display styles for trip estimates.

