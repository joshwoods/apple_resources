

- AVFoundation
-  AVAssetPlaybackAssistant 

Class

# AVAssetPlaybackAssistant

An object that provides playback information for an asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVAssetPlaybackAssistant
```

## Topics

### Creating a Playback Assistant

convenience init(asset: AVAsset)

Creates a playback assistant to inspect the specified asset.

### Loading Playback Configuration Options

func loadPlaybackConfigurationOptions(completionHandler: ([AVAssetPlaybackConfigurationOption]) -> Void)

Loads playback configuration options for an asset.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Utilities

struct AVAssetPlaybackConfigurationOption

A structure that defines playback configuration options for an asset.

