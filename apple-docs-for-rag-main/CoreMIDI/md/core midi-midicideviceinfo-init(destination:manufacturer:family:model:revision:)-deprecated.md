

- Core MIDI
- MIDICIDeviceInfo
-  init(destination:manufacturer:family:model:revision:) Deprecated

Initializer

# init(destination:manufacturer:family:model:revision:)

Creates a new device information instance.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(
    destination midiDestination: MIDIEntityRef,
    manufacturer: Data,
    family: Data,
    model modelNumber: Data,
    revision revisionLevel: Data
)
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`midiDestination`  

The MIDI destination to use for capability inquiry.

`manufacturer`  

The device manufacturer.

`family`  

The family to which this device belongs.

`modelNumber`  

The device’s model number.

`revisionLevel`  

The version of the device’s model number.

