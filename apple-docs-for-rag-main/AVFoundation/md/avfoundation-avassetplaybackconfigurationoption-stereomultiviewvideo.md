

- AVFoundation
- AVAssetPlaybackConfigurationOption
-  stereoMultiviewVideo 

Type Property

# stereoMultiviewVideo

An option that indicates whether the asset is in a multiview compression format and can render as stereo video.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let stereoMultiviewVideo: AVAssetPlaybackConfigurationOption
```

## Discussion

Apps may use this property to determine whether to configure stereo video rendering.

## See Also

### Configuration Options

static let stereoVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset can render as stereo video.

static let spatialVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset can render as spatial video.

