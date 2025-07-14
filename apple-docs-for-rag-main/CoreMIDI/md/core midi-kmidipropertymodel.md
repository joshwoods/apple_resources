

- Core MIDI
-  kMIDIPropertyModel 

Global Variable

# kMIDIPropertyModel

The model name of a device or endpoint.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyModel: CFString
```

## Discussion

Use this property in the following scenarios:

- MIDI drivers should set this property on their devices.

- Studio setup editors may allow the user to set this property on external devices.

- Creators of virtual endpoints may set this property on their endpoints.

## See Also

### Identification

let kMIDIPropertyName: CFString

A name for a device, entity, or endpoint.

let kMIDIPropertyManufacturer: CFString

The manufacturer name of a device or endpoint.

let kMIDIPropertyUniqueID: CFString

The unique identifier of a device, entity, or, endpoint.

let kMIDIPropertyDeviceID: CFString

The user-visible System Exclusive (SysEx) identifier of a device or entity.

