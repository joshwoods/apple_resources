

- AVFAudio
- AVAudioNode
-  name(forInputBus:) 

Instance Method

# name(forInputBus:)

Gets the name of the input bus you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func name(forInputBus bus: AVAudioNodeBus) -> String?
```

## Parameters 

`bus`  

The input bus from an audio node.

## Return Value

The name of the input bus.

## See Also

### Configuring an Input Format Bus

typealias AVAudioNodeBus

The index of a bus on an audio node.

func inputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Gets the input format for the bus you specify.

var numberOfInputs: Int

The number of input busses for the node.

