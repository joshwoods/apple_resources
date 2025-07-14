

- Audio Toolbox
- Audio Session Support
-  Audio Route Change Reasons 

API Collection

# Audio Route Change Reasons

Identifiers for the various reasons that an audio route can change while your app is running.

## Overview

You encounter these identifiers as values in the CFDictionary object passed to your property listener callback function when it is listening for audio route changes. See the description for kAudioSessionProperty_AudioRouteChange.

## Topics

### Constants

var kAudioSessionRouteChangeReason_Unknown: Int

The audio route changed but the reason is not known.

Deprecated

var kAudioSessionRouteChangeReason_NewDeviceAvailable: Int

A new audio hardware device became available; for example, a headset was plugged in.

var kAudioSessionRouteChangeReason_OldDeviceUnavailable: Int

The previously-used audio hardware device is now unavailable; for example, a headset was unplugged.

var kAudioSessionRouteChangeReason_CategoryChange: Int

The audio session category has changed.

var kAudioSessionRouteChangeReason_Override: Int

The audio route has been overridden.

var kAudioSessionRouteChangeReason_WakeFromSleep: Int

The device woke from sleep.

var kAudioSessionRouteChangeReason_NoSuitableRouteForCategory: Int

There is no audio hardware route for the audio session category.

var kAudioSessionRouteChangeReason_RouteConfigurationChange: Int

## See Also

### Audio Routes

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

