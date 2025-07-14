

- AVFoundation
-  AVAssetPlaybackConfigurationOption 

Structure

# AVAssetPlaybackConfigurationOption

A structure that defines playback configuration options for an asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AVAssetPlaybackConfigurationOption
```

## Topics

### Configuration Options

static let stereoVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset can render as stereo video.

static let stereoMultiviewVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset is in a multiview compression format and can render as stereo video.

static let spatialVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset can render as spatial video.

### Initializers

init(rawValue: String)

Creates a configuration option from its raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Utilities

class AVAssetPlaybackAssistant

An object that provides playback information for an asset.

