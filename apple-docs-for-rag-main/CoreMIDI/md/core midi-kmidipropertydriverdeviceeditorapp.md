

- Core MIDI
-  kMIDIPropertyDriverDeviceEditorApp 

Global Variable

# kMIDIPropertyDriverDeviceEditorApp

The full path to an app on the system that configures driver-owned devices.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.3+visionOS 1.0+

``` source
let kMIDIPropertyDriverDeviceEditorApp: CFString
```

## Discussion

Only drivers may set this property on their owned devices.

## See Also

### Configuration

let kMIDIPropertyNameConfigurationDictionary: CFString

The device’s current patch, note, and control name values in MIDINameDocument XML format.

let kMIDIPropertyMaxSysExSpeed: CFString

The maximum rate, in bytes per second, at which the system may reliably send System Exclusive (SysEx) messages to this object.

let kMIDIPropertyNameConfiguration: CFString

An XML representation of the device’s current patch, note, and control name values.

Deprecated

