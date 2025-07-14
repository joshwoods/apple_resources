

- AVFoundation
- AVCaptureAudioChannel
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the channel is in an enabled state.

macOS 10.7+

``` source
var isEnabled: Bool { get set }
```

## Discussion

By default, a connection enables all audio channels that it exposes. You can set this value to false to stop the flow of data for a particular channel.

## See Also

### Configuring a Channel

var volume: Float

The current volume (gain) of the channel.

