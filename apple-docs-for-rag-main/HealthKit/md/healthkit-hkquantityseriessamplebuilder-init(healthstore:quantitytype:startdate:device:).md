

- HealthKit
- HKQuantitySeriesSampleBuilder
-  init(healthStore:quantityType:startDate:device:) 

Initializer

# init(healthStore:quantityType:startDate:device:)

Creates a new quantity series builder.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    healthStore: HKHealthStore,
    quantityType: HKQuantityType,
    startDate: Date,
    device: HKDevice?
)
```

## Parameters 

`healthStore`  

The HealthKit store.

`quantityType`  

The sample’s quantity type.

`startDate`  

The sample’s start date.

`device`  

An object representing the device that provided the data. Pass `nil` if the app is generating its own data.

## See Also

### Creating a Quantity Series Builder

var quantityType: HKQuantityType

The quantity type for the series.

var startDate: Date

The starting date and time for the sample.

var device: HKDevice?

The device providing the data.

