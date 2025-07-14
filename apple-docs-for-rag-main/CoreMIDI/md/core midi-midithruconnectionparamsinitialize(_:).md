

- Core MIDI
-  MIDIThruConnectionParamsInitialize(\_:) 

Function

# MIDIThruConnectionParamsInitialize(\_:)

Initializes a parameters object with its default values.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionParamsInitialize(_ inConnectionParams: UnsafeMutablePointer)
```

## Parameters 

`inConnectionParams`  

The parameters to initialize.

## Discussion

This is a convenience function that fills the connection structure with default values. Set the source and destination to create a simple, unmodified thru connection.

## See Also

### Configuring Parameters

struct MIDIThruConnectionParams

A set of MIDI routings and transformations.

func MIDIThruConnectionParamsSize(UnsafePointer&lt;MIDIThruConnectionParams>) -> Int

Returns the size of a MIDI thru connection parameters object.

func MIDIThruConnectionGetParams(MIDIThruConnectionRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>>) -> OSStatus

Returns the thru connection’s parameters.

func MIDIThruConnectionSetParams(MIDIThruConnectionRef, CFData) -> OSStatus

Updates a thru connection’s parameters.

