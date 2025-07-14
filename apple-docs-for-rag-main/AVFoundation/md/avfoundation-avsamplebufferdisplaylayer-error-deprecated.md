

- AVFoundation
- AVSampleBufferDisplayLayer
-  error Deprecated

Instance Property

# error

The error that caused the failure.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var error: (any Error)? { get }
```

Deprecated

Use error on sampleBufferRenderer instead.

## Discussion

The value of this property is an `NSError` that describes what caused the display layer to no longer be able to enqueue sample buffers. If the status is not AVQueuedSampleBufferRenderingStatus.failed, the value of this property is `nil`.

