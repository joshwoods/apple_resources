

- Core MIDI
- MIDICIResponder
-  init(deviceInfo:profileDelegate:profileStates:supportProperties:) Deprecated

Initializer

# init(deviceInfo:profileDelegate:profileStates:supportProperties:)

Creates a new responder.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(
    deviceInfo: MIDICIDeviceInfo,
    profileDelegate delegate: any MIDICIProfileResponderDelegate,
    profileStates profileList: [MIDICIProfileState],
    supportProperties propertiesSupported: Bool
)
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`deviceInfo`  

The MIDI-CI device information.

`delegate`  

The responder’s delegate object.

`profileList`  

The list of profile state objects.

`propertiesSupported`  

A Boolean value that indicates whether the responder supports properties.

