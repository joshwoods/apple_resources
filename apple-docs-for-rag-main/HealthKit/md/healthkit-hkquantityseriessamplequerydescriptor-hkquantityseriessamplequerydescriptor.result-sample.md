

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
- HKQuantitySeriesSampleQueryDescriptor.Result
-  sample 

Instance Property

# sample

The quantity sample that owns the series of data entries.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
let sample: HKQuantitySample?
```

## Discussion

HealthKit sets this value to `nil` unless you included the includeSample option when you created the series query descriptor.

## See Also

### Accessing Sample Data

let quantity: HKQuantity

The quantity stored by the data entry.

let dateInterval: DateInterval

The date interval for the entry.

