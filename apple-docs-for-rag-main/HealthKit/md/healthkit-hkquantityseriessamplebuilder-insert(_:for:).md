

- HealthKit
- HKQuantitySeriesSampleBuilder
-  insert(\_:for:) 

Instance Method

# insert(\_:for:)

Adds a new quantity to the series with the provided date interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func insert(
    _ quantity: HKQuantity,
    for dateInterval: DateInterval
) throws
```

## Parameters 

`quantity`  

The quantity to insert.

`dateInterval`  

The date interval associated with the quantity. If the interval’s start parameter is the same as the start date for a previously provided quantity, this quantity replaces the previous one. This method fails with an HKError.Code.errorInvalidArgument error if the date parameter is earlier than the series builder’s startDate property.

## Discussion

Use this method to add a quantity to the series. The quantity must have a unit that is compatible with the series builder’s quantity type (see is(compatibleWith:)).

Note

You can insert quantities in any order. The builder sorts them by the date interval’s startDate property when you finish the series.

## See Also

### Adding Values

func insert(HKQuantity, at: Date) throws

Adds a new quantity to the series at the provided date and time.

