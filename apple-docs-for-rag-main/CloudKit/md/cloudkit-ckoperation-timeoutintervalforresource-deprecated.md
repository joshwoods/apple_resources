

- CloudKit
- CKOperation
-  timeoutIntervalForResource Deprecated

Instance Property

# timeoutIntervalForResource

The maximum amount of time that a resource request can use.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.13DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var timeoutIntervalForResource: TimeInterval { get set }
```

Deprecated

Use timeoutIntervalForResource instead.

## Discussion

This property determines the resource timeout interval for this operation, which controls how long, in seconds, to wait for the entire operation to complete before stopping. The resource timer starts when the operation executes and counts until either the operation completes or this timeout interval occurs, whichever comes first.

The default value is `604800`, the number of seconds in 7 days.

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

var timeoutIntervalForRequest: TimeInterval

The timeout interval when waiting for additional data.

Deprecated

