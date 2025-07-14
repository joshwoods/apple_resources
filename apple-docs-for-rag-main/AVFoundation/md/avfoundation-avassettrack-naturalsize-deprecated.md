

- AVFoundation
- AVAssetTrack
-  naturalSize Deprecated

Instance Property

# naturalSize

The natural dimensions of the media data that the track references.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var naturalSize: CGSize { get }
```

Deprecated

Load the value of naturalSize asynchronously instead.

## Discussion

For visual tracks, like video or subtitle tracks, this property value is the natural size of the media. For nonvisual tracks, like audio or chapter tracks, the value is zero.

