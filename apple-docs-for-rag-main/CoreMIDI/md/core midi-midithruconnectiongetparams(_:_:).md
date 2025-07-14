

- Core MIDI
-  MIDIThruConnectionGetParams(\_:\_:) 

Function

# MIDIThruConnectionGetParams(\_:\_:)

Returns the thru connection’s parameters.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionGetParams(
    _ connection: MIDIThruConnectionRef,
    _ outConnectionParams: UnsafeMutablePointer>
) -> OSStatus
```

## Parameters 

`connection`  

The connection to dispose.

`outConnectionParams`  

On successful return, the connection’s parameters in a CFData.

## Return Value

An `OSStatus` result code.

## Discussion

The returned object contains a MIDIThruConnectionParams structure. The caller is responsible for releasing it.

## See Also

### Configuring Parameters

struct MIDIThruConnectionParams

A set of MIDI routings and transformations.

func MIDIThruConnectionParamsSize(UnsafePointer&lt;MIDIThruConnectionParams>) -> Int

Returns the size of a MIDI thru connection parameters object.

func MIDIThruConnectionParamsInitialize(UnsafeMutablePointer&lt;MIDIThruConnectionParams>)

Initializes a parameters object with its default values.

func MIDIThruConnectionSetParams(MIDIThruConnectionRef, CFData) -> OSStatus

Updates a thru connection’s parameters.

