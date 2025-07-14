

- Core MIDI
- MIDICIDeviceInfo
-  family Deprecated

Instance Property

# family

The family to which the device belongs.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var family: Data { get }
```

Deprecated

No longer supported for CoreMIDI

## Discussion

This value is 2 bytes long.

## See Also

### Inspecting a Device

var manufacturerID: Data

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

Deprecated

var modelNumber: Data

The model number of the device.

Deprecated

var revisionLevel: Data

The revision number of the device model number.

Deprecated

var midiDestination: MIDIEndpointRef

The MIDI destination the device’s MIDI entity uses for capability inquiries.

Deprecated

