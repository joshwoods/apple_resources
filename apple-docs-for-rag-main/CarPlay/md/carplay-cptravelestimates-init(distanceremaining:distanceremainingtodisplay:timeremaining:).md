

- CarPlay
- CPTravelEstimates
-  init(distanceRemaining:distanceRemainingToDisplay:timeRemaining:) 

Initializer

# init(distanceRemaining:distanceRemainingToDisplay:timeRemaining:)

Creates a travel estimates instance with the distance remaining that the framework displays to a person.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
init(
    distanceRemaining: Measurement,
    distanceRemainingToDisplay: Measurement,
    timeRemaining time: TimeInterval
)
```

## Parameters 

`distanceRemaining`  

The distance remaining in `Measurement` units. distanceRemainingToDisplay: the disance remaining to dfisk to a person, in `Measurement` units. time: \`TimeInterval

## Return Value

A newly initialized travel estimates object.

## Discussion

If not set, falls back to `distanceRemaining`.

## See Also

### Creating a Travel Estimates Object

init(distanceRemaining: Measurement&lt;UnitLength>, timeRemaining: TimeInterval)

Creates travel estimates with the remaining distance and time.

