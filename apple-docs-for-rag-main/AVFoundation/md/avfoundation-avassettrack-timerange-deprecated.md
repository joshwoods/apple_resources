

- AVFoundation
- AVAssetTrack
-  timeRange Deprecated

Instance Property

# timeRange

The time range of the track within the overall timeline of the asset.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var timeRange: CMTimeRange { get }
```

Deprecated

Load the value of timeRange asynchronously instead.

## Discussion

If the start of the time range is greater than zero, the track doesn’t initially have media data to present. This condition may occur when the media delays an audio track to align the start of audio with a specific video frame. You can test for this as the example below shows:

- Swift
- Objective-C

```
if track.timeRange.start > .zero {
    // Delayed start.
}
```

```
if CMTIME_COMPARE_INLINE(track.timeRange.start, >, kCMTimeZero) {
    // Delayed start.
}
```

