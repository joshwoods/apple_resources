

- AVFoundation
- AVPlayerVideoOutput
- AVPlayerVideoOutput.Configuration
-  sourcePlayerItem 

Instance Property

# sourcePlayerItem

The player item that’s the source of this configuration.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
weak var sourcePlayerItem: AVPlayerItem? { get }
```

## See Also

### Inspecting the configuration

var dataChannelDescription: [[CMTag]]

An array of data channels selected for this configuration.

var activationTime: CMTime

The host time this configuration became active on its associated player object.

var preferredTransform: CGAffineTransform

The preferred transform of the visual media.

