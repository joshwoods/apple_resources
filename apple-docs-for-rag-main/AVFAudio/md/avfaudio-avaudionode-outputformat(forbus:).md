

- AVFAudio
- AVAudioNode
-  outputFormat(forBus:) 

Instance Method

# outputFormat(forBus:)

Retrieves the output format for the bus you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func outputFormat(forBus bus: AVAudioNodeBus) -> AVAudioFormat
```

## Parameters 

`bus`  

An audio node bus.

## Return Value

An AVAudioFormat instance that represents the output format of the bus.

## See Also

### Creating an Output Format Bus

func name(forOutputBus: AVAudioNodeBus) -> String?

Retrieves the name of the output bus you specify.

var numberOfOutputs: Int

The number of output busses for the node.

