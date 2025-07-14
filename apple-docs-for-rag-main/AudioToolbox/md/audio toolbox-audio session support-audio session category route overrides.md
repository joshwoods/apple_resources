

- Audio Toolbox
- Audio Session Support
-  Audio Session Category Route Overrides 

API Collection

# Audio Session Category Route Overrides

Specifies whether the default audio route for the `PlayAndRecord` category should be overridden.

## Overview

The `kAudioSessionCategory_PlayAndRecord` category supports simultaneous input and output. You could use this category, for example, to add an effect to audio coming into the device’s microphone. By default, output audio for this category goes to the receiver—the speaker you hold to your ear when on a phone call. The `kAudioSessionOverrideAudioRoute_Speaker` constant lets you direct the output audio to the speaker situated at the bottom of the phone.

## Topics

### Constants

var kAudioSessionOverrideAudioRoute_None: Int

Specifies, for the kAudioSessionCategory_PlayAndRecord category, that output audio should go to the receiver. This is the default output audio route for this category.

Deprecated

var kAudioSessionOverrideAudioRoute_Speaker: Int

Specifies, for the kAudioSessionCategory_PlayAndRecord category, that output audio should go to the speaker, not the receiver.

## See Also

### Audio Session Support

Audio Session Property Identifiers

Property identifiers used with Audio Session Services in iOS.

Audio Session Categories

Category identifiers for audio sessions, used as values for the kAudioSessionProperty_AudioCategory property.

Audio Session Modes

Mode identifiers for audio sessions, used as values for the kAudioSessionProperty_Mode property.

Audio Session Activation Flags

Flags that provide additional information about your app’s audio intentions upon session activation or deactivation.

Audio Session Interruption States

Identifiers used with the AudioSessionInterruptionListener callback function in iOS to indicate that an audio interruption has started or stopped.

typealias AudioSessionInterruptionType

Values that indicate the nature of the interruption that ended.

