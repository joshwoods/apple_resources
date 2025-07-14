

- HealthKit
- HKObjectType
-  seriesType(forIdentifier:) 

Type Method

# seriesType(forIdentifier:)

Returns the shared series type for the provided identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
class func seriesType(forIdentifier identifier: String) -> HKSeriesType?
```

## Parameters 

`identifier`  

A series type identifier. In iOS 11 and watchOS 4, there is only one series type identifier: HKWorkoutRouteTypeIdentifier.

## Return Value

The shared HKSeriesType instance based on the provided identifier.

## Discussion

This method returns an instance of the HKSeriesType concrete subclass. HealthKit uses series types to represent samples that store a series of items. You can’t directly instantiate these samples; instead, use a HKSeriesBuilder subclass to create them. Use series types to ask for permission to read series data from the HealthKit store.

## See Also

### Related Documentation

class func workoutRoute() -> Self

Returns a series type object for workout routes.

class HKWorkoutRoute

A sample that contains a workout’s route data.

class HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

