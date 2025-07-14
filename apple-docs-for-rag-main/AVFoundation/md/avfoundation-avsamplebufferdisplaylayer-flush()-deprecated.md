

- AVFoundation
- AVSampleBufferDisplayLayer
-  flush() Deprecated

Instance Method

# flush()

Instructs the layer to discard any enqueued sample buffers that are pending.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func flush()
```

Deprecated

Use sampleBufferRenderer's flush instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use flush() on the sampleBufferRenderer instead.

Because it’s not possible to determine which sample buffers have been decoded, the next frame passed to enqueue(_:) should be an IDR frame (also known as a key frame or sync sample).

## See Also

### Flushing Sample Buffers

func flushAndRemoveImage()

Instructs the layer to discard pending enqueued sample buffers and remove any currently displayed image.

Deprecated

