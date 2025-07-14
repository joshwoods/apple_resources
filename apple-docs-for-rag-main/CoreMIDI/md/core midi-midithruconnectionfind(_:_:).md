

- Core MIDI
-  MIDIThruConnectionFind(\_:\_:) 

Function

# MIDIThruConnectionFind(\_:\_:)

Finds the persistent thru connections for the specified client.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIThruConnectionFind(
    _ inPersistentOwnerID: CFString,
    _ outConnectionList: UnsafeMutablePointer>
) -> OSStatus
```

## Parameters 

`inPersistentOwnerID`  

The identifier of the owning object.

`outConnectionList`  

On successful return, a CFData that contains an array of MIDI thru connections.

## Return Value

An `OSStatus` result code.

