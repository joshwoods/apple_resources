

- Core MIDI
-  MIDIThruConnectionParamsSize(\_:) 

Function

# MIDIThruConnectionParamsSize(\_:)

Returns the size of a MIDI thru connection parameters object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDIThruConnectionParamsSize(_ ptr: UnsafePointer) -> Int
```

## Parameters 

`ptr`  

The parameters pointer.

## Return Value

The connection’s parameter’s size.

## Discussion

This function accounts for variable-length elements in the structure and returns its true size in bytes.

## See Also

### Configuring Parameters

struct MIDIThruConnectionParams

A set of MIDI routings and transformations.

func MIDIThruConnectionParamsInitialize(UnsafeMutablePointer&lt;MIDIThruConnectionParams>)

Initializes a parameters object with its default values.

func MIDIThruConnectionGetParams(MIDIThruConnectionRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>>) -> OSStatus

Returns the thru connection’s parameters.

func MIDIThruConnectionSetParams(MIDIThruConnectionRef, CFData) -> OSStatus

Updates a thru connection’s parameters.

