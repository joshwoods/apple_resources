

- AVFoundation
- AVPlayerItem
-  variantPreferences 

Instance Property

# variantPreferences

The preferences the player item uses when selecting variant playlists.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
nonisolated
var variantPreferences: AVVariantPreferences { get set }
```

## Discussion

The default value is AVVariantPreferenceNone.

Note

Changing variant preferences during playback might result in a variant switch.

## See Also

### Setting Variant Behavior

struct AVVariantPreferences

Defines the preferences the player item uses when selecting variant playlists.

var startsOnFirstEligibleVariant: Bool

A Boolean value that indicates whether playback starts with the first eligible variant that appears in the stream’s main playlist.

