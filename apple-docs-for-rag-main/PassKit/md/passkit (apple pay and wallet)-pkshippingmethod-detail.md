

- PassKit (Apple Pay and Wallet)
- PKShippingMethod
-  detail 

Instance Property

# detail

A user-readable description of the shipping method.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var detail: String? { get set }
```

## Discussion

Use this property to differentiate the shipping methods you offer. For example “Ships in 24 hours.” or “Arrives by 5pm on July 29.”

Don’t repeat the content of the label property inherited from PKPaymentSummaryItem.

Note

When dateComponentsRange contains a value, the system displays the range in the shipping method panel of the payment sheet. The system displays the contents of detail on the shipping method selection pane.

## See Also

### Working with shipping methods

var dateComponentsRange: PKDateComponentsRange?

An expected range of delivery or shipping dates for a package, or the time range when an item is available for pickup.

var identifier: String?

A unique identifier for the shipping method, used by the app.

class PKDateComponentsRange

An object that specifies the start and end dates for a range of time.

