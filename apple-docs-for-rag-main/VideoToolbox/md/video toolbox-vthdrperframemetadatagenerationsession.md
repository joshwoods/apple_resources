

- Video Toolbox
-  VTHDRPerFrameMetadataGenerationSession 

Class

# VTHDRPerFrameMetadataGenerationSession

An object that generates per-frame HDR metadata.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class VTHDRPerFrameMetadataGenerationSession
```

## Topics

### Creating a session

init(framesPerSecond: Float, hdrFormats: [VTHDRPerFrameMetadataGenerationSession.HDRFormat]?) throws

### Attaching metadata

func attachMetadata(to: CVPixelBuffer, sceneChange: Bool) throws

### HDR Formats

enum HDRFormat

