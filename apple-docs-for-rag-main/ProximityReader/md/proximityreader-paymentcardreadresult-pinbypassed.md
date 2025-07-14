

- ProximityReader
- PaymentCardReadResult
-  pinBypassed 

Instance Property

# pinBypassed

A Boolean value that indicates whether the consumer bypassed the PIN entry.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
let pinBypassed: Bool
```

## Discussion

When the framework sets this property to `false`, the consumer didn’t bypass the PIN entry or it wasn’t required.

## See Also

### Getting the PIN status

let isPINFallback: Bool

A Boolean value that indicates whether the PIN Fallback occurred.

