

- AVFoundation
- AVAssetTrack
-  preferredVolume Deprecated

Instance Property

# preferredVolume

The track’s volume preference for playing its audible media.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var preferredVolume: Float { get }
```

Deprecated

Load the value of preferredVolume asynchronously instead.

## Discussion

The preferred volume for an audio track is typically, but not always, `1.0`. For non-audible tracks, the value is `0.0`.

