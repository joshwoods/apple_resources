

- PassKit (Apple Pay and Wallet)
- PKShippingMethod
-  identifier 

Instance Property

# identifier

A unique identifier for the shipping method, used by the app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var identifier: String? { get set }
```

## Discussion

This property isn’t user visible.

Use this property of the shipping method passed to your delegate in the paymentAuthorizationViewController(_:didSelect:completion:) method to identify the chosen shipping method.

## See Also

### Working with shipping methods

var detail: String?

A user-readable description of the shipping method.

var dateComponentsRange: PKDateComponentsRange?

An expected range of delivery or shipping dates for a package, or the time range when an item is available for pickup.

class PKDateComponentsRange

An object that specifies the start and end dates for a range of time.

