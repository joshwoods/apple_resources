

- AVFoundation
- AVSampleBufferDisplayLayer
-  status Deprecated

Instance Property

# status

The ability of the display layer to be used for enqueuing sample buffers.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.10–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var status: AVQueuedSampleBufferRenderingStatus { get }
```

Deprecated

Use sampleBufferRenderer's status instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use status on sampleBufferRenderer instead.

The value of this property is an AVQueuedSampleBufferRenderingStatus that indicates whether the receiver can be used for enqueuing sample buffers.

When the value of this property is AVQueuedSampleBufferRenderingStatus.failed, the receiver can no longer be used and a new instance needs to be created in its place. When this happens, clients can check the value of the error property to determine the failure.

This property supports key-value observing.

## See Also

### Getting Display Layer Settings

enum AVQueuedSampleBufferRenderingStatus

The statuses for sample buffer rendering.

