

- CloudKit
- CKOperation
-  timeoutIntervalForRequest Deprecated

Instance Property

# timeoutIntervalForRequest

The timeout interval when waiting for additional data.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.13DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var timeoutIntervalForRequest: TimeInterval { get set }
```

Deprecated

Use timeoutIntervalForRequest instead.

## Discussion

This property determines the request timeout interval for the operation, which controls how long, in seconds, the operation waits for additional data to arrive before stopping. The timer for this value resets whenever new data arrives. When the timer reaches the interval without receiving any new data, it triggers a timeout.

The default value is `60`.

## See Also

### Deprecated Properties

var allowsCellularAccess: Bool

A Boolean value that indicates whether the operation can send data over the cellular network.

Deprecated

var container: CKContainer?

The operation’s container.

Deprecated

var isLongLived: Bool

A Boolean value that indicates whether the operation is long-lived.

Deprecated

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request can use.

Deprecated

