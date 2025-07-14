

- Core MIDI
-  kMIDIPropertyNameConfiguration Deprecated

Global Variable

# kMIDIPropertyNameConfiguration

An XML representation of the device’s current patch, note, and control name values.

iOS 4.2–13.0DeprecatediPadOS 4.2–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let kMIDIPropertyNameConfiguration: CFString
```

Deprecated

Use kMIDIPropertyNameConfigurationDictionary instead.

## See Also

### Configuration

let kMIDIPropertyNameConfigurationDictionary: CFString

The device’s current patch, note, and control name values in MIDINameDocument XML format.

let kMIDIPropertyMaxSysExSpeed: CFString

The maximum rate, in bytes per second, at which the system may reliably send System Exclusive (SysEx) messages to this object.

let kMIDIPropertyDriverDeviceEditorApp: CFString

The full path to an app on the system that configures driver-owned devices.

