

- AVFAudio
-  AVAudioUnitSampler 

Class

# AVAudioUnitSampler

An object that you configure with one or more instrument samples, based on Apple’s Sampler audio unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitSampler
```

## Overview

An `AVAudioUnitSampler` is an AVAudioUnit for Apple’s Sampler audio unit.

You configure the sampler by loading instruments from different types of files. These include an `aupreset` file, DLS, or SF2 sound bank; an EXS24 instrument; a single audio file; or an array of audio files.

The output of a `AVAudioUnitSampler` is a single stereo bus.

## Topics

### Configuring the Sampler Audio Unit

func loadInstrument(at: URL) throws

Configures the sampler with the specified instrument file.

func loadAudioFiles(at: [URL]) throws

Configures the sampler by loading the specified audio files.

func loadSoundBankInstrument(at: URL, program: UInt8, bankMSB: UInt8, bankLSB: UInt8) throws

Loads a specific instrument from the specified soundbank.

### Getting and Setting Sampler Values

var globalTuning: Float

An adjustment for the tuning of all the played notes.

var overallGain: Float

An adjustment for the gain of all the played notes, in decibels.

var stereoPan: Float

An adjustment for the stereo panning of all the played notes.

var masterGain: Float

An adjustment for the gain of all the played notes, in decibels.

Deprecated

## Relationships

### Inherits From

- AVAudioUnitMIDIInstrument

### Conforms To

- AVAudio3DMixing
- AVAudioMixing
- AVAudioStereoMixing
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### MIDI

class AVAudioSequencer

An object that plays audio from a collection of MIDI events the system organizes into music tracks.

