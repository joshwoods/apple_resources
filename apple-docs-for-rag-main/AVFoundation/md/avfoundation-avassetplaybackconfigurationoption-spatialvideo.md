

- AVFoundation
- AVAssetPlaybackConfigurationOption
-  spatialVideo 

Type Property

# spatialVideo

An option that indicates whether the asset can render as spatial video.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static let spatialVideo: AVAssetPlaybackConfigurationOption
```

## Discussion

Apps may use this property to determine whether to configure spatial video rendering.

## See Also

### Configuration Options

static let stereoVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset can render as stereo video.

static let stereoMultiviewVideo: AVAssetPlaybackConfigurationOption

An option that indicates whether the asset is in a multiview compression format and can render as stereo video.

