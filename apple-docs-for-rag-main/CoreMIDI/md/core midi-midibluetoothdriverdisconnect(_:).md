

- Core MIDI
-  MIDIBluetoothDriverDisconnect(\_:) 

Function

# MIDIBluetoothDriverDisconnect(\_:)

Disconnect the Bluetooth MIDI driver from a Bluetooth Low Energy MIDI peripheral.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func MIDIBluetoothDriverDisconnect(_ uuid: CFString) -> OSStatus
```

## Parameters 

`uuid`  

A unique identifier that represents the peripheral to disconnect.

## Return Value

A status code that indicates the result of the disconnect.

## Discussion

If a Core MIDI device is in a connected state to a Bluetooth Low Energy MIDI peripheral with the identifier you specify, the system disconnects it.

## See Also

### Managing Device Connections

func MIDIBluetoothDriverActivateAllConnections() -> OSStatus

Promote all active Bluetooth connections into an online MIDI device capable of input and output.

