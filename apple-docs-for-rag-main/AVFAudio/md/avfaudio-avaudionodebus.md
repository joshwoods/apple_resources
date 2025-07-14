

- AVFAudio
-  AVAudioNodeBus 

Type Alias

# AVAudioNodeBus

The index of a bus on an audio node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAudioNodeBus = Int
```

## Discussion

An AVAudioNodeBus represents a bus as a zero-based index. AVAudioNode objects potentially have multiple input and output busses.

## See Also

### Configuring an Input Format Bus

func inputFormat(forBus: AVAudioNodeBus) -> AVAudioFormat

Gets the input format for the bus you specify.

func name(forInputBus: AVAudioNodeBus) -> String?

Gets the name of the input bus you specify.

var numberOfInputs: Int

The number of input busses for the node.

