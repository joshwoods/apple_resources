

- HealthKit
- HKWorkoutRouteBuilder
-  init(healthStore:device:) 

Initializer

# init(healthStore:device:)

Creates and returns a new workout route builder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    healthStore: HKHealthStore,
    device: HKDevice?
)
```

## Parameters 

`healthStore`  

The HealthKit store.

`device`  

An object representing the device that provided the location data. Pass `nil` if the app is generating its own location data (for example, using Core Location).

## Return Value

A newly initialized workout route builder.

