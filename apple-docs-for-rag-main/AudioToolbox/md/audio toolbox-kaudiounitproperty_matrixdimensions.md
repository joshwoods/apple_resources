

- Audio Toolbox
-  kAudioUnitProperty_MatrixDimensions 

Global Variable

# kAudioUnitProperty_MatrixDimensions

Indicates the total number of channels for input and output of a given matrix mixer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioUnitProperty_MatrixDimensions: AudioUnitPropertyID { get }
```

## Discussion

A read-only `2 * UInt32` value valid on the audio unit global scope.

## See Also

### Constants

var kAudioUnitProperty_InputAnchorTimeStamp: AudioUnitPropertyID

var kAudioUnitProperty_MatrixLevels: AudioUnitPropertyID

Describes the internal state of a matrix mixer.

var kAudioUnitProperty_MeterClipping: AudioUnitPropertyID

Indicates audio clipping that has occurred since this property was last accessed.

var kAudioUnitProperty_MeteringMode: AudioUnitPropertyID

Specifies whether metering is enabled or disabled for a particular scope-element combination.

