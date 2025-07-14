

- CloudKit
- CKOperation
-  isLongLived Deprecated

Instance Property

# isLongLived

A Boolean value that indicates whether the operation is long-lived.

iOS 9.3–11.0DeprecatediPadOS 9.3–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.13DeprecatedtvOS 9.2–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–4.0Deprecated

``` source
var isLongLived: Bool { get set }
```

Deprecated

Use isLongLived instead.

## Discussion

Set this property to true to make the operation long-lived. The default value is false. If you change this property’s value after you execute the operation, the change has no effect.

For more information, see Long-Lived Operations.

## See Also

### Deprecated Properties

var allowsCellularAccess: Bool

A Boolean value that indicates whether the operation can send data over the cellular network.

Deprecated

var container: CKContainer?

The operation’s container.

Deprecated

var timeoutIntervalForRequest: TimeInterval

The timeout interval when waiting for additional data.

Deprecated

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request can use.

Deprecated

