

- HealthKit
- HKQuantitySeriesSampleBuilder
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Adds a new quantity to the series at the provided date and time.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
func insert(
    _ quantity: HKQuantity,
    at date: Date
) throws
```

## Parameters 

`quantity`  

The quantity to insert.

`date`  

The start date associated with the quantity. If this is the same start date as a previously provided quantity, this quantity replaces the previous one. This method fails with an HKError.Code.errorInvalidArgument error if the `date` parameter is earlier than the series builder’s startDate property.

## Discussion

This method calls insert(_:for:), passing a date interval with the provided start date, and a duration of `0`.

## See Also

### Adding Values

func insert(HKQuantity, for: DateInterval) throws

Adds a new quantity to the series with the provided date interval.

