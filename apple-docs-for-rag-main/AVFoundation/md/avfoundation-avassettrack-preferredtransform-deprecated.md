

- AVFoundation
- AVAssetTrack
-  preferredTransform Deprecated

Instance Property

# preferredTransform

The track’s transform preference to apply to its visual content during presentation or processing.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var preferredTransform: CGAffineTransform { get }
```

Deprecated

Load the value of preferredTransform asynchronously instead.

## Discussion

The value of this property is typically, but not always, CGAffineTransformIdentity.

