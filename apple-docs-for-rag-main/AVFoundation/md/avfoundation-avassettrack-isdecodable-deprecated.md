

- AVFoundation
- AVAssetTrack
-  isDecodable Deprecated

Instance Property

# isDecodable

A Boolean value that indicates whether the track is decodable in the current environment.

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.13–13.0DeprecatedtvOS 11.0–16.0DeprecatedwatchOS 4.0–9.0Deprecated

``` source
var isDecodable: Bool { get }
```

Deprecated

Load the value of isDecodable asynchronously instead.

## Discussion

When this property is true, the system can decode the track, even if decoding may be too slow for real-time playback.

