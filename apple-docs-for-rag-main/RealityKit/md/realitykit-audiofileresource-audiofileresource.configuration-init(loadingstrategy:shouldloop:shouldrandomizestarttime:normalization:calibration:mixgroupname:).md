

- RealityKit
- AudioFileResource
- AudioFileResource.Configuration
-  init(loadingStrategy:shouldLoop:shouldRandomizeStartTime:normalization:calibration:mixGroupName:) 

Initializer

# init(loadingStrategy:shouldLoop:shouldRandomizeStartTime:normalization:calibration:mixGroupName:)

Initializes a new audio file resource configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    loadingStrategy: AudioFileResource.LoadingStrategy = .preload,
    shouldLoop: Bool = false,
    shouldRandomizeStartTime: Bool = false,
    normalization: AudioResource.Normalization? = nil,
    calibration: AudioResource.Calibration? = nil,
    mixGroupName: String? = nil
)
```

