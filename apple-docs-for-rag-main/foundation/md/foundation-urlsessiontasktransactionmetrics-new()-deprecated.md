

- Foundation
- URLSessionTaskTransactionMetrics
-  new() Deprecated

Type Method

# new()

Creates a new transaction metrics instance.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.15DeprecatedtvOS 10.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–6.0Deprecated

``` source
class func new() -> Self
```

Deprecated

Not supported

## Discussion

You should never need to create your own URLSessionTaskTransactionMetrics instances. The URLSession creates task transaction metrics as part of the URLSessionTaskMetrics instance that it delivers to the urlSession(_:task:didFinishCollecting:) method of URLSessionTaskDelegate.

## See Also

### Creating transaction metrics

init()

Creates a transaction metrics instance.

Deprecated

