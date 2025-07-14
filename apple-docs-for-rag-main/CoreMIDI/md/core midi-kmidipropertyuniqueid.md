

- Core MIDI
-  kMIDIPropertyUniqueID 

Global Variable

# kMIDIPropertyUniqueID

The unique identifier of a device, entity, or, endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyUniqueID: CFString
```

## Discussion

The system assigns unique IDs to all objects. You may set this property on virtual endpoints; however, doing so may fail if the ID isn’t unique.

This property value is an integer.

## See Also

### Identification

let kMIDIPropertyName: CFString

A name for a device, entity, or endpoint.

let kMIDIPropertyModel: CFString

The model name of a device or endpoint.

let kMIDIPropertyManufacturer: CFString

The manufacturer name of a device or endpoint.

let kMIDIPropertyDeviceID: CFString

The user-visible System Exclusive (SysEx) identifier of a device or entity.

