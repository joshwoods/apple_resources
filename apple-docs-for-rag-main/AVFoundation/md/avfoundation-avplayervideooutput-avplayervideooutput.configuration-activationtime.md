

- AVFoundation
- AVPlayerVideoOutput
- AVPlayerVideoOutput.Configuration
-  activationTime 

Instance Property

# activationTime

The host time this configuration became active on its associated player object.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
var activationTime: CMTime { get }
```

## See Also

### Inspecting the configuration

var sourcePlayerItem: AVPlayerItem?

The player item that’s the source of this configuration.

var dataChannelDescription: [[CMTag]]

An array of data channels selected for this configuration.

var preferredTransform: CGAffineTransform

The preferred transform of the visual media.

