

- Audio Toolbox
-  kAudioOutputUnitProperty_EnableIO 

Global Variable

# kAudioOutputUnitProperty_EnableIO

Specifies whether audio I/O is enabled for an I/O unit bus-scope combination.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioOutputUnitProperty_EnableIO: AudioUnitPropertyID { get }
```

## Discussion

An I/O unit’s bus 0 connects to output hardware, such as for playback through a speaker. Output is enabled by default. To disable output, the bus 0 output scope must be disabled, as follows:

```
UInt32 enableOutput        = 0;    // to disable output
AudioUnitElement outputBus = 0;

AudioUnitSetProperty (
    io_unit_instance,
    kAudioOutputUnitProperty_EnableIO,
    kAudioUnitScope_Output,
    outputBus,
    &enableOutput,
    sizeof (enableOutput)
);
```

An I/O unit’s bus 1 connects to input hardware, such as for recording from a microphone. Input is disabled by default. To enable input, the bus 1 input scope must be enabled, as follows:

```
UInt32 enableInput        = 1;    // to enable input
AudioUnitElement inputBus = 1;

AudioUnitSetProperty (
    io_unit_instance,
    kAudioOutputUnitProperty_EnableIO,
    kAudioUnitScope_Input,
    inputBus,
    &enableInput,
    sizeof (enableInput)
);
```

A read/write `UInt32` value valid on the input and output scopes.

## See Also

### Properties

var kAudioOutputUnitProperty_ChannelMap: AudioUnitPropertyID

var kAudioOutputUnitProperty_CurrentDevice: AudioUnitPropertyID

A read/write audio device ID object, of type `AudioDeviceID`, valid on the audio unit global scope.

var kAudioOutputUnitProperty_HasIO: AudioUnitPropertyID

var kAudioOutputUnitProperty_SetInputCallback: AudioUnitPropertyID

A read/write `AURenderCallbackStruct` data structure valid on the audio unit global scope. When an output unit has been enabled for input operation, this callback can be used to provide a single callback to the host application from the input I/O proc, in order to notify the host that input is available and may be obtained by calling the `AudioUnitRender` function.

var kAudioOutputUnitProperty_StartTime: AudioUnitPropertyID

A write-only `AudioOutputUnitStartAtTimeParams` data structure valid on the audio unit global scope. When this property is set on an output unit, it will cause the next Start request (but no subsequent Starts) to use the AudioDeviceStartAtTime function, using the specified timestamp, passing false for `inRequestedStartTimeIsInput`.

var kAudioOutputUnitProperty_StartTimestampsAtZero: AudioUnitPropertyID

A read/write `UInt32` value valid on the audio unit global scope.

var kAudioOutputUnitProperty_IsRunning: AudioUnitPropertyID

Indicates whether an audio unit is running (`TRUE`) or not (`FALSE`).

