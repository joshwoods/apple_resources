

- Core MIDI
-  MIDIThruConnectionSetParams(\_:\_:) 

Function

# MIDIThruConnectionSetParams(\_:\_:)

Updates a thru connection’s parameters.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionSetParams(
    _ connection: MIDIThruConnectionRef,
    _ inConnectionParams: CFData
) -> OSStatus
```

## Parameters 

`connection`  

The connection to update.

`inConnectionParams`  

The connection’s new parameters in a CFData.

## Return Value

An `OSStatus` result code.

## See Also

### Configuring Parameters

struct MIDIThruConnectionParams

A set of MIDI routings and transformations.

func MIDIThruConnectionParamsSize(UnsafePointer&lt;MIDIThruConnectionParams>) -> Int

Returns the size of a MIDI thru connection parameters object.

func MIDIThruConnectionParamsInitialize(UnsafeMutablePointer&lt;MIDIThruConnectionParams>)

Initializes a parameters object with its default values.

func MIDIThruConnectionGetParams(MIDIThruConnectionRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>>) -> OSStatus

Returns the thru connection’s parameters.

