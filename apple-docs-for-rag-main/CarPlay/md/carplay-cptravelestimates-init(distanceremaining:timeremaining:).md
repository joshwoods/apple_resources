

- CarPlay
- CPTravelEstimates
-  init(distanceRemaining:timeRemaining:) 

Initializer

# init(distanceRemaining:timeRemaining:)

Creates travel estimates with the remaining distance and time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    distanceRemaining distance: Measurement,
    timeRemaining time: TimeInterval
)
```

## Parameters 

`distance`  

The remaining distance for the travel estimate.

`time`  

The remaining time for the travel estimate.

## Return Value

A newly initialized travel estimates object.

## See Also

### Creating a Travel Estimates Object

init(distanceRemaining: Measurement&lt;UnitLength>, distanceRemainingToDisplay: Measurement&lt;UnitLength>, timeRemaining: TimeInterval)

Creates a travel estimates instance with the distance remaining that the framework displays to a person.

