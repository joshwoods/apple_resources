

- AVFoundation
- AVPlayerVideoOutput
- AVPlayerVideoOutput.Configuration
-  dataChannelDescription 

Instance Property

# dataChannelDescription

An array of data channels selected for this configuration.

iOS 17.2+iPadOS 17.2+Mac CatalystmacOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
var dataChannelDescription: [[CMTag]] { get }
```

## See Also

### Inspecting the configuration

var sourcePlayerItem: AVPlayerItem?

The player item that’s the source of this configuration.

var activationTime: CMTime

The host time this configuration became active on its associated player object.

var preferredTransform: CGAffineTransform

The preferred transform of the visual media.

