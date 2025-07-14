

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentSummaryItem
-  intervalUnit 

Instance Property

# intervalUnit

The amount of time – in calendar units such as day, month, or year – that represents a fraction of the total payment interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
var intervalUnit: NSCalendar.Unit { get set }
```

## Discussion

The default value for the interval unit is month.

The supported NSCalendar.Unit interval units are:

- minute

- hour

- day

- month

- year

To set an interval unit based on a week, set intervalUnit to day, and set intervalCount to a multiple of the number of days per week. To find the number of days for a week in the current calendar, call `NSCalendar.current.maximumRange(of: .weekday)!.count)`.

For example, the code below sets a payment that occurs every two weeks.

```
let daysPerWeek = NSCalendar.current.maximumRange(of: .weekday)!.count)

intervalUnit = .day
intervalCount = daysPerWeek * 2
```

## See Also

### Setting the payment interval

var intervalCount: Int

The number of interval units that make up the total payment interval.

