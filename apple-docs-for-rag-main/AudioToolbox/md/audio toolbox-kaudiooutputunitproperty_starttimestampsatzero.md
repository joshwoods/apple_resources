

- Audio Toolbox
-  kAudioOutputUnitProperty_StartTimestampsAtZero 

Global Variable

# kAudioOutputUnitProperty_StartTimestampsAtZero

A read/write `UInt32` value valid on the audio unit global scope.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioOutputUnitProperty_StartTimestampsAtZero: AudioUnitPropertyID { get }
```

## See Also

### Properties

var kAudioOutputUnitProperty_ChannelMap: AudioUnitPropertyID

var kAudioOutputUnitProperty_CurrentDevice: AudioUnitPropertyID

A read/write audio device ID object, of type `AudioDeviceID`, valid on the audio unit global scope.

var kAudioOutputUnitProperty_EnableIO: AudioUnitPropertyID

Specifies whether audio I/O is enabled for an I/O unit bus-scope combination.

var kAudioOutputUnitProperty_HasIO: AudioUnitPropertyID

var kAudioOutputUnitProperty_SetInputCallback: AudioUnitPropertyID

A read/write `AURenderCallbackStruct` data structure valid on the audio unit global scope. When an output unit has been enabled for input operation, this callback can be used to provide a single callback to the host application from the input I/O proc, in order to notify the host that input is available and may be obtained by calling the `AudioUnitRender` function.

var kAudioOutputUnitProperty_StartTime: AudioUnitPropertyID

A write-only `AudioOutputUnitStartAtTimeParams` data structure valid on the audio unit global scope. When this property is set on an output unit, it will cause the next Start request (but no subsequent Starts) to use the AudioDeviceStartAtTime function, using the specified timestamp, passing false for `inRequestedStartTimeIsInput`.

var kAudioOutputUnitProperty_IsRunning: AudioUnitPropertyID

Indicates whether an audio unit is running (`TRUE`) or not (`FALSE`).

