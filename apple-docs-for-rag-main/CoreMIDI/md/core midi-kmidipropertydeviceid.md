

- Core MIDI
-  kMIDIPropertyDeviceID 

Global Variable

# kMIDIPropertyDeviceID

The user-visible System Exclusive (SysEx) identifier of a device or entity.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyDeviceID: CFString
```

## Discussion

MIDI drivers can set this property on their devices or entities. Studio setup editors can allow the user to set this property on external devices.

## See Also

### Identification

let kMIDIPropertyName: CFString

A name for a device, entity, or endpoint.

let kMIDIPropertyModel: CFString

The model name of a device or endpoint.

let kMIDIPropertyManufacturer: CFString

The manufacturer name of a device or endpoint.

let kMIDIPropertyUniqueID: CFString

The unique identifier of a device, entity, or, endpoint.

