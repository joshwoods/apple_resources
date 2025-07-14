

- AVFAudio
- AVAudioNode
-  name(forOutputBus:) 

Instance Method

# name(forOutputBus:)

Retrieves the name of the output bus you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func name(forOutputBus bus: AVAudioNodeBus) -> String?
```

## Parameters 

`bus`  

The output bus from an audio node.

## Return Value

The name of the output bus.

## See Also

### Creating an Output Format Bus

func outputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Retrieves the output format for the bus you specify.

var numberOfOutputs: Int

The number of output busses for the node.

