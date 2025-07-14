

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentSummaryItem
-  intervalCount 

Instance Property

# intervalCount

The number of interval units that make up the total payment interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
var intervalCount: Int { get set }
```

## Discussion

The default value is `1`, which requests a recurring payment every one intervalUnit.

## See Also

### Setting the payment interval

var intervalUnit: NSCalendar.Unit

The amount of time – in calendar units such as day, month, or year – that represents a fraction of the total payment interval.

