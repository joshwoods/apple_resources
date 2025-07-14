

- Audio Toolbox
- Audio Unit Properties
-  I/O Audio Unit Function Selectors 

API Collection

# I/O Audio Unit Function Selectors

Audio unit component selectors, specific to I/O audio units, that correspond to functions in the audio unit API.

## Topics

### Constants

var kAudioOutputUnitRange: Int

The start of the numerical range for I/O audio unit function selectors.

var kAudioOutputUnitStartSelect: Int

Used by the system to start an I/O audio unit when you call the AudioOutputUnitStart(_:) function.

var kAudioOutputUnitStopSelect: Int

Used by the system to stop an I/O audio unit when you call the AudioOutputUnitStop(_:) function.

## See Also

### Input/Output

I/O Audio Unit Properties

Properties for Apple I/O audio units (sometimes called output units).

Inter-App Output Unit Property IDs

Inter-App Audio Unit Property IDs

Output Unit Parameters

AUNetReceive Properties

AUNetSend Properties

AUNetSend Parameters

AUNetReceive Parameters

AUNetSendPresetFormat Properties

Net Status Audio Unit Parameters

struct AudioOutputUnitMIDICallbacks

struct AudioOutputUnitStartAtTimeParams

A timestamp for scheduled starting of an I/O audio unit.

