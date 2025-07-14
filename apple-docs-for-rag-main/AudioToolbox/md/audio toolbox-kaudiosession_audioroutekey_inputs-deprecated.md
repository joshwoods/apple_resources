

- Audio Toolbox
-  kAudioSession_AudioRouteKey_Inputs Deprecated

Global Variable

# kAudioSession_AudioRouteKey_Inputs

An object containing details about audio input used in the current audio route.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let kAudioSession_AudioRouteKey_Inputs: CFString!
```

Deprecated

Deprecated in iOS 7.0.

## Discussion

If there is an audio input available, the array contains a CFDictionary object with a single key, namely kAudioSession_AudioRouteKey_Type, whose value is one of the constants in Audio Input Routes.

If no audio input is available, the array is empty.

## See Also

### Constants

let kAudioSessionInputRoute_BluetoothHFP: CFString!

A microphone that is part of a Bluetooth Hands-Free Profile (HFP) device.

Deprecated

let kAudioSessionInputRoute_BuiltInMic: CFString!

A built-in microphone input.

Deprecated

let kAudioSessionInputRoute_HeadsetMic: CFString!

A microphone that is part of a headset.

Deprecated

let kAudioSessionInputRoute_LineIn: CFString!

A line in input

Deprecated

let kAudioSessionInputRoute_USBAudio: CFString!

A Universal Serial Bus (USB) input, accessed through the device 30-pin connector.

Deprecated

let kAudioSessionOutputRoute_AirPlay: CFString!

An output on an AirPlay device.

Deprecated

let kAudioSessionOutputRoute_BluetoothA2DP: CFString!

Speakers in a Bluetooth A2DP device.

Deprecated

let kAudioSessionOutputRoute_BluetoothHFP: CFString!

Speakers that are part of a Bluetooth Hands-Free Profile (HFP) accessory.

Deprecated

let kAudioSessionOutputRoute_BuiltInReceiver: CFString!

The built-in speaker you hold to your ear when on a phone call.

Deprecated

let kAudioSessionOutputRoute_BuiltInSpeaker: CFString!

The primary built-in speaker.

Deprecated

let kAudioSessionOutputRoute_HDMI: CFString!

An output available through the HDMI interface.

Deprecated

let kAudioSessionOutputRoute_Headphones: CFString!

Speakers in headphones or in a headset.

Deprecated

let kAudioSessionOutputRoute_LineOut: CFString!

Analog line-level output.

Deprecated

let kAudioSessionOutputRoute_USBAudio: CFString!

Speaker(s) in a Universal Serial Bus (USB) accessory, accessed through the device 30-pin connector.

Deprecated

let kAudioSession_AudioRouteChangeKey_CurrentRouteDescription: CFString!

Describes the current audio route.

Deprecated

