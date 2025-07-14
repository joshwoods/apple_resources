

- AVFoundation
-  AVVariantPreferences 

Structure

# AVVariantPreferences

Defines the preferences the player item uses when selecting variant playlists.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
struct AVVariantPreferences
```

## Topics

### Preference Settings

static var scalabilityToLosslessAudio: AVVariantPreferences

A preference that indicates the player item supports variant playlists that contain losslessly encoded audio when sufficient bandwidth is available.

### Initializers

init(rawValue: UInt)

Creates a variant preferences structure with an integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Setting Variant Behavior

var variantPreferences: AVVariantPreferences

The preferences the player item uses when selecting variant playlists.

var startsOnFirstEligibleVariant: Bool

A Boolean value that indicates whether playback starts with the first eligible variant that appears in the stream’s main playlist.

