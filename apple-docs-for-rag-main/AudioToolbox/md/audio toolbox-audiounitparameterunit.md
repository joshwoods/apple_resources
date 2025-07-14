

- Audio Toolbox
-  AudioUnitParameterUnit 

Enumeration

# AudioUnitParameterUnit

The unit-of-measure for an audio unit parameter.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum AudioUnitParameterUnit
```

## Overview

The various units of measure for audio unit parameters are described in `Audio Unit Parameter Units of Measure`.

## Topics

### Enumeration Cases

case absoluteCents

An absolute unit of measure for the musical pitch of a note.

case BPM

A whole-number unit of measure for musical tempo, representing beats per minute.

case beats

A time unit of measure in musical beats.

case boolean

A Boolean-like unit of measure.

case cents

A logarithmic unit of measure for a musical interval between two notes.

case customUnit

A custom unit of measure.

case decibels

A logarithmic unit of measure representing the ratio between two audio levels.

case degrees

An angular degree unit of measure.

case equalPowerCrossfade

An audio power unit of measure.

case generic

A generic unit of measure.

case hertz

A hertz unit of measure.

case indexed

An indexed unit of measure.

case linearGain

A linear unit of measure representing the difference between two audio levels.

case midiController

A whole-number unit of measure corresponding to standard MIDI control numbers.

case midiNoteNumber

A whole-number unit of measure corresponding to audio frequency.

case meters

A distance unit of measure, corresponding to meters.

case milliseconds

A time unit of measure representing milliseconds.

case mixerFaderCurve1

An audio power unit of measure.

case octaves

A relative unit of measure for the musical interval between two notes.

case pan

An audio position unit of measure.

case percent

A percentage unit of measure.

case phase

An angular degree unit of measure.

case rate

A multiplication factor unit of measure.

case ratio

A unitless ratio unit of measure.

case relativeSemiTones

A relative unit of measure for a musical interval between two notes.

case sampleFrames

A sample-frame-count unit of measure.

case seconds

A whole-seconds unit of measure, indicating either absolute or relative time.

case midi2Controller

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

Audio Unit Types

The defined types of audio processing plug-ins known as audio units.

Inter-App Audio Unit Types

Audio Unit Manufacturer Identifier

The Apple audio unit manufacturer code.

Audio Unit Output Subtypes

I/O Audio Unit Subtypes

Converter Audio Unit Subtypes

Audio data format converter audio unit subtypes for audio units provided by Apple.

Reserved Audio Unit Clump Identifier

Reserved for system use.

Offline Audio Unit Properties

Properties for audio units that perform offline processing—that is, processing in a nonplayback, nonrealtime mode.

MIDI Audio Unit Parameters

Parameters for instrument units.

General Audio Unit Function Selectors

General audio unit component selectors that correspond to functions in the audio unit API.

Generator Audio Unit Subtypes

Audio units that serve as sound sources.

Input/Output Audio Unit Subtypes

Input/output audio unit subtypes for audio units provided by Apple.

Audio Unit Panner Subtypes

Audio Unit Player Subtypes

Audio Unit Pitch Subtypes

