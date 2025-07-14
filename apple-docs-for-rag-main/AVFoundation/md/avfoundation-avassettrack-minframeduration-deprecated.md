

- AVFoundation
- AVAssetTrack
-  minFrameDuration Deprecated

Instance Property

# minFrameDuration

The minimum duration of the track’s frames.

iOS 7.0–16.0DeprecatediPadOS 7.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var minFrameDuration: CMTime { get }
```

Deprecated

Load the value of minFrameDuration asynchronously instead.

## Discussion

A track’s minimum frame duration is the reciprocal of its maximum frame rate. For example, a video track with a maximum frame rate of 30 frames per second has a minimum frame duration of 1/30, or 0.033 seconds.

The value of this property is invalid if the track can’t calculate its minimum frame duration, or if it’s unknown.

