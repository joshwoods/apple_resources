

- AVFoundation
- AVAsset
-  minimumTimeOffsetFromLive Deprecated

Instance Property

# minimumTimeOffsetFromLive

A time value that indicates how closely playback follows the latest live stream content.

iOS 13.0–16.0DeprecatediPadOS 13.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.15–13.0DeprecatedtvOS 13.0–16.0DeprecatedwatchOS 6.0–9.0Deprecated

``` source
var minimumTimeOffsetFromLive: CMTime { get }
```

Deprecated

Load the value of minimumTimeOffsetFromLive asynchronously instead.

## Discussion

This property value is only valid when working with live streaming content. For non-live assets, this property value is invalid.

