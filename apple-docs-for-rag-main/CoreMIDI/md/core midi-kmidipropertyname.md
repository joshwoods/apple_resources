

- Core MIDI
-  kMIDIPropertyName 

Global Variable

# kMIDIPropertyName

A name for a device, entity, or endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyName: CFString
```

## Discussion

Devices, entities, and endpoints may all have names. The standard way to display an endpoint’s name is to ask it for its name and display it only if unique. If not, prepend the device name.

A studio setup editor may allow the user to set the names of both driver-owned and external devices.

## See Also

### Identification

let kMIDIPropertyModel: CFString

The model name of a device or endpoint.

let kMIDIPropertyManufacturer: CFString

The manufacturer name of a device or endpoint.

let kMIDIPropertyUniqueID: CFString

The unique identifier of a device, entity, or, endpoint.

let kMIDIPropertyDeviceID: CFString

The user-visible System Exclusive (SysEx) identifier of a device or entity.

