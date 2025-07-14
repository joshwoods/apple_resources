

- Audio Toolbox
-  Audio Session Support 

API Collection

# Audio Session Support

Describe the properties that you associate with audio sessions and audio routes.

## Overview

Important

The `AudioSession` API has been completely deprecated in iOS 7.0. See AVAudioSession for the Objective-C implementation of these functions.

Audio Session Services lets you specify the intended audio behavior for your iOS app. For example, you can specify whether you intend for your app’s audio to silence other apps or to mix with their audio. You also use this API to specify your app’s behavior when it is interrupted, such as by a phone call. When the system knows your intentions, it configures the audio hardware in the device to satisfy those intentions, as possible.

These functions apply only to iOS. They do not apply to macOS.

## Topics

### Audio Session Support

Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

### Audio Routes

Audio Route Change Reasons

Identifiers for the various reasons that an audio route can change while your app is running.

Audio Route Description Dictionary Keys

Keys for the kAudioSessionProperty_AudioRouteDescription dictionary.

Audio Route Type Key

The one key for an audio route input or output dictionary.

Audio Input Routes

Strings that identify the various audio input sources for a device.

Audio Output Routes

The various audio output destinations available for an iOS device.

Audio Route Change Dictionary Keys

Keys for obtaining information about an audio hardware route change.

Alternative Audio Route Change Reason Dictionary Key

An alternate key for obtaining information about the reason for an audio route change.

### USB Accessories

USB Accessory Audio Source Dictionary Keys

Keys for the dictionaries in the kAudioSessionProperty_InputSources array.

USB Accessory Audio Destination Dictionary Keys

Keys for the dictionaries in the kAudioSessionProperty_OutputDestinations array.

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

let kAudioSession_AudioRouteChangeKey_PreviousRouteDescription: CFString!

Describes the previous audio route.

Deprecated

let kAudioSession_AudioRouteKey_Inputs: CFString!

An object containing details about audio input used in the current audio route.

Deprecated

let kAudioSession_AudioRouteKey_Outputs: CFString!

An object containing details about the audio output used in the current audio route.

Deprecated

let kAudioSession_AudioRouteKey_Type: CFString!

Audio routes input or output dictionary.

Deprecated

let kAudioSession_InputSourceKey_Description: CFString!

Audio input source description.

Deprecated

let kAudioSession_InputSourceKey_ID: CFString!

An audio input source.

Deprecated

let kAudioSession_OutputDestinationKey_Description: CFString!

The audio output destination.

Deprecated

let kAudioSession_OutputDestinationKey_ID: CFString!

The output destination.

Deprecated

let kAudioSession_RouteChangeKey_Reason: CFString!

The reason for the audio route change.

Deprecated

### Enumerations

Audio Session Interruption Types

### Result Codes

Audio Session Errors

## See Also

### Utilities

Analyzing audio performance with Instruments

Ensure a smooth and immersive audio experience in your apps using Audio System Trace.

Audio Converter Services

Convert between linear PCM audio formats, and between linear PCM and compressed formats.

Audio Toolbox Debugging

Obtain the internal state of Core Audio objects during the development and debugging of your code.

Workgroup Management

Coordinate the activity of custom real-time audio threads with those of the system and other processes.

Audio Codec

Translate audio data from one format to another.

Clock Utilities

Manage time-related information associated with audio playback.

