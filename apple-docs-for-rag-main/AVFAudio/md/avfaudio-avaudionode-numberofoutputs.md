

- AVFAudio
- AVAudioNode
-  numberOfOutputs 

Instance Property

# numberOfOutputs

The number of output busses for the node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var numberOfOutputs: Int { get }
```

## See Also

### Creating an Output Format Bus

func outputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Retrieves the output format for the bus you specify.

func name(forOutputBus: AVAudioNodeBus) -> String?

Retrieves the name of the output bus you specify.

