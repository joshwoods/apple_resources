

- Foundation
- URLSessionTaskMetrics
-  init() Deprecated

Initializer

# init()

Creates a task metrics instance.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.15DeprecatedtvOS 10.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–6.0Deprecated

``` source
init()
```

Deprecated

Not supported

## Discussion

You should never need to create your own URLSessionTaskMetrics instances. If you are interested in task metrics, implement the urlSession(_:task:didFinishCollecting:) method of URLSessionTaskDelegate. The URLSession will collect task metrics for you and deliver them to this method.

