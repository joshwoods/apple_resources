

- AVFoundation
- AVAssetPlaybackAssistant
-  loadPlaybackConfigurationOptions(completionHandler:) 

Instance Method

# loadPlaybackConfigurationOptions(completionHandler:)

Loads playback configuration options for an asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func loadPlaybackConfigurationOptions(completionHandler: @escaping ([AVAssetPlaybackConfigurationOption]) -> Void)
```

``` source
var playbackConfigurationOptions: [AVAssetPlaybackConfigurationOption] { get async }
```

## Parameters 

`completionHandler`  

A callback the system invokes with an array of AVAssetPlaybackConfigurationOption values that describe capabilities of the asset.

