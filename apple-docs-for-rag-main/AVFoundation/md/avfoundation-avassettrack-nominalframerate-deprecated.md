

- AVFoundation
- AVAssetTrack
-  nominalFrameRate Deprecated

Instance Property

# nominalFrameRate

The frame rate of the track, in frames per second.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var nominalFrameRate: Float { get }
```

Deprecated

Load the value of nominalFrameRate asynchronously instead.

## Discussion

The nominal frame rate indicates the number of frames per second for tracks that contain a full frame per media sample. For field-based (interlaced) video tracks, the value of this property indicates the field rate, not the frame rate.

