

- Core MIDI
-  kMIDIPropertyMaxSysExSpeed 

Global Variable

# kMIDIPropertyMaxSysExSpeed

The maximum rate, in bytes per second, at which the system may reliably send System Exclusive (SysEx) messages to this object.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
let kMIDIPropertyMaxSysExSpeed: CFString
```

## Discussion

The owning driver may set an integer value for this property.

## See Also

### Configuration

let kMIDIPropertyNameConfigurationDictionary: CFString

The device’s current patch, note, and control name values in MIDINameDocument XML format.

let kMIDIPropertyDriverDeviceEditorApp: CFString

The full path to an app on the system that configures driver-owned devices.

let kMIDIPropertyNameConfiguration: CFString

An XML representation of the device’s current patch, note, and control name values.

Deprecated

