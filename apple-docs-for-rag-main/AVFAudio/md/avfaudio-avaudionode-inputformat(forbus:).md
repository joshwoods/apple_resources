

- AVFAudio
- AVAudioNode
-  inputFormat(forBus:) 

Instance Method

# inputFormat(forBus:)

Gets the input format for the bus you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func inputFormat(forBus bus: AVAudioNodeBus) -> AVAudioFormat
```

## Parameters 

`bus`  

An audio node bus.

## Return Value

An AVAudioFormat instance that represents the input format of the bus.

## See Also

### Related Documentation

AVFoundation Programming Guide

### Configuring an Input Format Bus

typealias AVAudioNodeBus

The index of a bus on an audio node.

func name(forInputBus: AVAudioNodeBus) -> String?

Gets the name of the input bus you specify.

var numberOfInputs: Int

The number of input busses for the node.

