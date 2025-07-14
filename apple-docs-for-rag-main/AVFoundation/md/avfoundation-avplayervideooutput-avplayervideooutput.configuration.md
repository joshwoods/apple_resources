

- AVFoundation
- AVPlayerVideoOutput
-  AVPlayerVideoOutput.Configuration 

Class

# AVPlayerVideoOutput.Configuration

An object that provides configuration information for the related player item.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
class Configuration
```

## Topics

### Inspecting the configuration

var sourcePlayerItem: AVPlayerItem?

The player item that’s the source of this configuration.

var dataChannelDescription: [[CMTag]]

An array of data channels selected for this configuration.

var activationTime: CMTime

The host time this configuration became active on its associated player object.

var preferredTransform: CGAffineTransform

The preferred transform of the visual media.

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

## See Also

### Accessing video data

func taggedBuffers(forHostTime: CMTime) -> (taggedBufferGroup: [CMTaggedBuffer], presentationTime: CMTime, activeConfiguration: AVPlayerVideoOutput.Configuration)?

