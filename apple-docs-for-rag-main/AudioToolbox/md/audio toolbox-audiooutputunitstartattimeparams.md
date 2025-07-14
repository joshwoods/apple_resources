

- Audio Toolbox
-  AudioOutputUnitStartAtTimeParams 

Structure

# AudioOutputUnitStartAtTimeParams

A timestamp for scheduled starting of an I/O audio unit.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioOutputUnitStartAtTimeParams
```

## Topics

### Initializers

init()

init(mTimestamp: AudioTimeStamp, mFlags: UInt32)

### Instance Properties

var mFlags: UInt32

var mTimestamp: AudioTimeStamp

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

struct AudioOutputUnitMIDICallbacks

