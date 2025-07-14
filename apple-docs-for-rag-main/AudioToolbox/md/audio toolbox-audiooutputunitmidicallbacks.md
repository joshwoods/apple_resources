

- Audio Toolbox
-  AudioOutputUnitMIDICallbacks 

Structure

# AudioOutputUnitMIDICallbacks

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioOutputUnitMIDICallbacks
```

## Topics

### Initializers

init(userData: UnsafeMutableRawPointer?, MIDIEventProc: (UnsafeMutableRawPointer?, UInt32, UInt32, UInt32, UInt32) -> Void, MIDISysExProc: (UnsafeMutableRawPointer?, UnsafePointer&lt;UInt8>, UInt32) -> Void)

### Instance Properties

var MIDIEventProc: (UnsafeMutableRawPointer?, UInt32, UInt32, UInt32, UInt32) -> Void

var MIDISysExProc: (UnsafeMutableRawPointer?, UnsafePointer&lt;UInt8>, UInt32) -> Void

var userData: UnsafeMutableRawPointer?

## Relationships

### Conforms To

- BitwiseCopyable

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

I/O Audio Unit Function Selectors

Audio unit component selectors, specific to I/O audio units, that correspond to functions in the audio unit API.

struct AudioOutputUnitStartAtTimeParams

A timestamp for scheduled starting of an I/O audio unit.

