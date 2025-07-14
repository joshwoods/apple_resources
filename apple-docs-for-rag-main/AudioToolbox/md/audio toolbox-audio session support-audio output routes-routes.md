

- Audio Toolbox
- Audio Session Support
-  Audio Output Routes 

API Collection

# Audio Output Routes

The various audio output destinations available for an iOS device.

## Overview

These strings are used as values for the kAudioSession_AudioRouteKey_Type key for the dictionary associated with the kAudioSession_AudioRouteKey_Outputs array.

## Topics

### Constants

let kAudioSessionOutputRoute_LineOut: CFString!

Analog line-level output.

Deprecated

let kAudioSessionOutputRoute_Headphones: CFString!

Speakers in headphones or in a headset.

Deprecated

let kAudioSessionOutputRoute_BluetoothHFP: CFString!

Speakers that are part of a Bluetooth Hands-Free Profile (HFP) accessory.

Deprecated

let kAudioSessionOutputRoute_BluetoothA2DP: CFString!

Speakers in a Bluetooth A2DP device.

Deprecated

let kAudioSessionOutputRoute_BuiltInReceiver: CFString!

The built-in speaker you hold to your ear when on a phone call.

Deprecated

let kAudioSessionOutputRoute_BuiltInSpeaker: CFString!

The primary built-in speaker.

Deprecated

let kAudioSessionOutputRoute_USBAudio: CFString!

Speaker(s) in a Universal Serial Bus (USB) accessory, accessed through the device 30-pin connector.

Deprecated

let kAudioSessionOutputRoute_HDMI: CFString!

An output available through the HDMI interface.

Deprecated

let kAudioSessionOutputRoute_AirPlay: CFString!

An output on an AirPlay device.

Deprecated

## See Also

### Audio Routes

Audio Route Change Reasons

Identifiers for the various reasons that an audio route can change while your app is running.

Audio Route Description Dictionary Keys

Keys for the kAudioSessionProperty_AudioRouteDescription dictionary.

Audio Route Type Key

The one key for an audio route input or output dictionary.

Audio Input Routes

Strings that identify the various audio input sources for a device.

Audio Route Change Dictionary Keys

Keys for obtaining information about an audio hardware route change.

Alternative Audio Route Change Reason Dictionary Key

An alternate key for obtaining information about the reason for an audio route change.

