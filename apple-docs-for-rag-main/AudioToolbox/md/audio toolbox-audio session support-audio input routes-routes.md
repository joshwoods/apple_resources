

- Audio Toolbox
- Audio Session Support
-  Audio Input Routes 

API Collection

# Audio Input Routes

Strings that identify the various audio input sources for a device.

## Overview

These strings are used as values for the kAudioSession_AudioRouteKey_Type key for the dictionary associated with the kAudioSession_AudioRouteKey_Inputs array.

## Topics

### Constants

let kAudioSessionInputRoute_LineIn: CFString!

A line in input

Deprecated

let kAudioSessionInputRoute_BuiltInMic: CFString!

A built-in microphone input.

Deprecated

let kAudioSessionInputRoute_HeadsetMic: CFString!

A microphone that is part of a headset.

Deprecated

let kAudioSessionInputRoute_BluetoothHFP: CFString!

A microphone that is part of a Bluetooth Hands-Free Profile (HFP) device.

Deprecated

let kAudioSessionInputRoute_USBAudio: CFString!

A Universal Serial Bus (USB) input, accessed through the device 30-pin connector.

Deprecated

## See Also

### Audio Routes

Audio Route Change Reasons

Identifiers for the various reasons that an audio route can change while your app is running.

Audio Route Description Dictionary Keys

Keys for the kAudioSessionProperty_AudioRouteDescription dictionary.

Audio Route Type Key

The one key for an audio route input or output dictionary.

Audio Output Routes

The various audio output destinations available for an iOS device.

Audio Route Change Dictionary Keys

Keys for obtaining information about an audio hardware route change.

Alternative Audio Route Change Reason Dictionary Key

An alternate key for obtaining information about the reason for an audio route change.

