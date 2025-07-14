

- Core Services
- Apple Events
- AESendMode
-  kAEWantReceipt 

Global Variable

# kAEWantReceipt

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAEWantReceipt: Int { get }
```

## Discussion

Deprecated and unsupported in macOS. The return receipt preference—the sender wants to receive a return receipt for this Apple event from the Event Manager. (A return receipt means only that the receiving application accepted the Apple event the Apple event may or may not be handled successfully after it is accepted.) If the receiving application does not send a return receipt before the request times out, `AESend` returns `errAETimeout` as its function result.

