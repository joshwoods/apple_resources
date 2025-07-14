

- StoreKit
- SKPaymentQueue
-  default() Deprecated

Type Method

# default()

Returns the default payment queue instance.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class func `default`() -> Self
```

Deprecated

No longer supported

## Return Value

The default payment queue.

## Discussion

Apps do not create a payment queue. Instead, they retrieve the queue by calling this class method.

### Special Considerations

The payment queue is not available in Simulator. Attempting to retrieve the payment queue logs a warning.

