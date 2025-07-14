

- HealthKit
- HKDiscreteQuantitySample
-  mostRecentQuantity 

Instance Property

# mostRecentQuantity

The most recent quantity contained by the sample.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var mostRecentQuantity: HKQuantity { get }
```

## Discussion

The sample sorts its contained quantities based on the startDate property for the quantity’s date interval.

## See Also

### Accessing Calculated Values

var averageQuantity: HKQuantity

The average of all quantities contained by the sample.

var maximumQuantity: HKQuantity

The maximum quantity contained by the sample.

var minimumQuantity: HKQuantity

The minimum value contained by the sample.

var mostRecentQuantityDateInterval: DateInterval

The date interval for the most recent quantity contained by the sample.

