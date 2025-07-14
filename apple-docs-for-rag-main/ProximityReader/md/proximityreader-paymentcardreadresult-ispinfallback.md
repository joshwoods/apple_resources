

- ProximityReader
- PaymentCardReadResult
-  isPINFallback 

Instance Property

# isPINFallback

A Boolean value that indicates whether the PIN Fallback occurred.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
let isPINFallback: Bool
```

## Discussion

When the framework sets this property to `true`, the `paymentCardData` is a PIN Fallback read.

## See Also

### Getting the PIN status

let pinBypassed: Bool

A Boolean value that indicates whether the consumer bypassed the PIN entry.

