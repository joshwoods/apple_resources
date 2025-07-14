

- AVFoundation
- AVAsset
-  isPlayable Deprecated

Instance Property

# isPlayable

A Boolean value that indicates whether the asset has playable content.

iOS 4.3–16.0DeprecatediPadOS 4.3–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var isPlayable: Bool { get }
```

Deprecated

Load the value of isPlayable asynchronously instead.

## Discussion

This property value is true if you can use the asset to create an AVPlayerItem.

