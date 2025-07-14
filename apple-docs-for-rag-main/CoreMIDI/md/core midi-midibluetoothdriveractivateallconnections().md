

- Core MIDI
-  MIDIBluetoothDriverActivateAllConnections() 

Function

# MIDIBluetoothDriverActivateAllConnections()

Promote all active Bluetooth connections into an online MIDI device capable of input and output.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func MIDIBluetoothDriverActivateAllConnections() -> OSStatus
```

## Return Value

A status code that indicates the result of the activation.

## Discussion

To establish a Bluetooth MIDI driver connection to a Bluetooth Low Energy (BLE) MIDI peripheral, perform the following steps:

1.  Scan for the peripheral’s advertised BLE MIDI service by using Core Bluetooth.

2.  Connect to the advertised peripheral by using Core Bluetooth.

3.  Call MIDIBluetoothDriverActivateAllConnections() upon successful connection.

4.  Confirm the peripheral’s registration by using Core MIDI and inspecting MIDIDeviceRef.

If the device reference is present, Core MIDI owns a connection to the peripheral, so use Core Bluetooth to disconnect from the peripheral.

## See Also

### Managing Device Connections

func MIDIBluetoothDriverDisconnect(CFString) -> OSStatus

Disconnect the Bluetooth MIDI driver from a Bluetooth Low Energy MIDI peripheral.

