

- Core Location
- CLActivityType
-  CLActivityType.automotiveNavigation 

Case

# CLActivityType.automotiveNavigation

The value that indicates positioning in an automobile following a road network.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case automotiveNavigation
```

## Mentioned in 

Getting the current location of a device

## Discussion

Use this activity type when your app is using the location manager specifically during a vehicular positioning session to track location changes to the automobile.

This activity might cause the system to pause location updates when the vehicle doesn’t move for an extended period of time.

## See Also

### Activity types

case other

The value that indicates the app is using location manager for an unspecified activity.

case fitness

The value that indicates positioning during dedicated fitness sessions, such as walking workouts, running workouts, cycling workouts, and so on.

case otherNavigation

The value that indicates positioning for activities that don’t or may not adhere to roads such as cycling, scooters, trains, boats and off-road vehicles.

case airborne

The value that indicates activities in the air.

