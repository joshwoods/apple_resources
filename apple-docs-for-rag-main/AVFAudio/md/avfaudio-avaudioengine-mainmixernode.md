

- AVFAudio
- AVAudioEngine
-  mainMixerNode 

Instance Property

# mainMixerNode

The audio engine’s optional singleton main mixer node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mainMixerNode: AVAudioMixerNode { get }
```

## Discussion

The audio engine constructs a singleton main mixer and connects it to the outputNode when first accessing this property. You can then connect additional audio nodes to the mixer.

If the client never sets the connection format between the `mainMixerNode` and the `outputNode`, the engine always updates the format to track the format of the `outputNode` on startup or restart, even after an AVAudioEngineConfigurationChangeNotification. Otherwise, it’s the client’s responsibility to update the connection format after an AVAudioEngineConfigurationChangeNotification.

By default, the mixer’s output format (sample rate and channel count) tracks the format of the output node.

## See Also

### Getting the Input, Output, and Main Mixer Nodes

var inputNode: AVAudioInputNode

The audio engine’s singleton input audio node.

var outputNode: AVAudioOutputNode

The audio engine’s singleton output audio node.

