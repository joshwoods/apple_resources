

- Core MIDI
-  MIDIDeviceCreate(\_:\_:\_:\_:\_:) 

Function

# MIDIDeviceCreate(\_:\_:\_:\_:\_:)

Creates a new device object that corresponds to the available hardware.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceCreate(
    _ owner: MIDIDriverRef?,
    _ name: CFString,
    _ manufacturer: CFString,
    _ model: CFString,
    _ outDevice: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`owner`  

The driver that creates the device, or `NULL` for a non-driver.

`name`  

The name of the new device.

`manufacturer`  

The name of the device’s manufacturer.

`model`  

The name of the model of the device.

`outDevice`  

On successful return, points to the newly created device.

## Return Value

An `OSStatus` result code.

## Discussion

Nondrivers may call this function to create external devices.

## See Also

### Managing Device Lifecyle

func MIDIDeviceDispose(MIDIDeviceRef) -> OSStatus

Disposes of a MIDI device.

typealias MIDIDeviceRef

A MIDI device that contains entities.

