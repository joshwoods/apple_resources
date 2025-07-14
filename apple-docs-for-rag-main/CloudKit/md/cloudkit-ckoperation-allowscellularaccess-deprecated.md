

- CloudKit
- CKOperation
-  allowsCellularAccess Deprecated

Instance Property

# allowsCellularAccess

A Boolean value that indicates whether the operation can send data over the cellular network.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var allowsCellularAccess: Bool { get set }
```

Deprecated

Use allowsCellularAccess instead.

## Discussion

When you send or receive many records, or when you send records with large assets, you might set this property to false to avoid consuming too much of the user’s cellular data bandwidth. The default value is true.

When this property is false, the operation fails if Wi-Fi isn’t available.

## See Also

### Deprecated Properties

var container: CKContainer?

The operation’s container.

Deprecated

var isLongLived: Bool

A Boolean value that indicates whether the operation is long-lived.

Deprecated

var timeoutIntervalForRequest: TimeInterval

The timeout interval when waiting for additional data.

Deprecated

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request can use.

Deprecated

