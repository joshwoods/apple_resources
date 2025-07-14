

- ProximityReader
- PaymentCardReader
- PaymentCardReader.Options
-  vasMerchants Deprecated

Instance Property

# vasMerchants

A global list of merchants to use when reading loyalty cards.

iOS 15.4–18.0DeprecatediPadOS 15.4–18.0DeprecatedMac Catalyst 17.0–18.0Deprecated

``` source
var vasMerchants: [VASRequest.Merchant]
```

Deprecated

Use VASRequest to specify VAS merchants

## Discussion

When you try to read a loyalty card from your PaymentCardReaderSession object, specify a custom VASRequest object to override this list.

