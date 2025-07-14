

- Audio Toolbox
- Audio Unit Properties
-  I/O Audio Unit Properties 

API Collection

# I/O Audio Unit Properties

Properties for Apple I/O audio units (sometimes called output units).

## Topics

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

var kAudioOutputUnitProperty_StartTimestampsAtZero: AudioUnitPropertyID

A read/write `UInt32` value valid on the audio unit global scope.

var kAudioOutputUnitProperty_IsRunning: AudioUnitPropertyID

Indicates whether an audio unit is running (`TRUE`) or not (`FALSE`).

## See Also

### Input/Output

Inter-App Output Unit Property IDs

Inter-App Audio Unit Property IDs

Output Unit Parameters

AUNetReceive Properties

AUNetSend Properties

AUNetSend Parameters

AUNetReceive Parameters

AUNetSendPresetFormat Properties

Net Status Audio Unit Parameters

I/O Audio Unit Function Selectors

Audio unit component selectors, specific to I/O audio units, that correspond to functions in the audio unit API.

struct AudioOutputUnitMIDICallbacks

struct AudioOutputUnitStartAtTimeParams

A timestamp for scheduled starting of an I/O audio unit.

