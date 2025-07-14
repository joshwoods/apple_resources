

- AVFoundation
- AVPlayerItem
-  timedMetadata Deprecated

Instance Property

# timedMetadata

An array of the most recently encountered timed metadata.

iOS 4.0–13.0DeprecatediPadOS 4.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var timedMetadata: [AVMetadataItem]? { get }
```

Deprecated

Use AVPlayerItemMetadataOutput to access timed metadata.

## Return Value

An array of AVMetadataItem or `nil` if no metadata was found.

## Discussion

Prior to the player item loading its media, this property value is `nil`. You can key-value observe this property to monitor when metadata becomes available.

