

- AVFoundation
- AVSampleBufferDisplayLayer
-  timebase Deprecated

Instance Property

# timebase

The renderer’s timebase, which determines how the layer interprets time stamps.

iOS 8.0–18.0DeprecatediPadOS 8.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 10.2–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var timebase: CMTimebase { get }
```

Deprecated

Use sampleBufferRenderer's timebase instead

## Discussion

Apple discourages the use of this symbol in iOS 17, tvOS 17, and macOS 14 and later. Use timebase on the sampleBufferRenderer instead.

