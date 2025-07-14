

- Core Location
- CLActivityType
-  CLActivityType.fitness 

Case

# CLActivityType.fitness

The value that indicates positioning during dedicated fitness sessions, such as walking workouts, running workouts, cycling workouts, and so on.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case fitness
```

## Discussion

For other positioning sessions that aren’t workouts, use CLActivityType.otherNavigation or CLActivityType.other. This activity might cause the system to pause location updates when the user doesn’t move a significant distance over a period of time.

When activityType is CLActivityType.fitness, the system disables indoor positioning.

## See Also

### Activity types

case other

The value that indicates the app is using location manager for an unspecified activity.

case automotiveNavigation

The value that indicates positioning in an automobile following a road network.

case otherNavigation

The value that indicates positioning for activities that don’t or may not adhere to roads such as cycling, scooters, trains, boats and off-road vehicles.

case airborne

The value that indicates activities in the air.

