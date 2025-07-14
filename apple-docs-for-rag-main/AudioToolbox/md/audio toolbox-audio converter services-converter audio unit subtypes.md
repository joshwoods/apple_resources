

- Audio Toolbox
- Audio Converter Services
-  Converter Audio Unit Subtypes 

API Collection

# Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

## Topics

### Constants

var kAudioUnitSubType_AUConverter: UInt32

var kAudioUnitSubType_AUiPodTimeOther: UInt32

var kAudioUnitSubType_DeferredRenderer: UInt32

var kAudioUnitSubType_Merger: UInt32

var kAudioUnitSubType_MultiSplitter: UInt32

var kAudioUnitSubType_NewTimePitch: UInt32

var kAudioUnitSubType_RoundTripAAC: UInt32

var kAudioUnitSubType_Splitter: UInt32

var kAudioUnitSubType_Varispeed: UInt32

An audio unit that can control playback rate. As the playback rate increases, so does pitch. This subtype provides a generic view, making it suitable for UI and programmatic context. macOS provides realtime and offline audio units of this subtype.

## See Also

### Enumerations

Converter Audio Unit Properties

Properties for the Apple AUConverter audio unit.

Audio Converter Dithering Algorithms

Audio Converter Properties (macOS)

Audio Converter Errors

