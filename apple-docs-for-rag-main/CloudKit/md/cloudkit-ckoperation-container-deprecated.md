

- CloudKit
- CKOperation
-  container Deprecated

Instance Property

# container

The operation’s container.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var container: CKContainer? { get set }
```

Deprecated

Use container instead.

## Discussion

The container defines where the operation executes. The add(_:) method of the CKContainer and CKDatabase classes implicitly set this property to their container.

If you execute the operation yourself, either directly or using a custom operation queue, set the value of this property explicitly. If the value is `nil` when you execute an operation, the operation implicitly executes in your app’s default container.

## See Also

### Deprecated Properties

var allowsCellularAccess: Bool

A Boolean value that indicates whether the operation can send data over the cellular network.

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

