

- Audio Toolbox
- AudioUnitParameterUnit
-  AudioUnitParameterUnit.absoluteCents 

Case

# AudioUnitParameterUnit.absoluteCents

An absolute unit of measure for the musical pitch of a note.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case absoluteCents
```

## Discussion

Absolute musical pitch in cents. 1,200 cents are equal to one octave. If `f` is a frequency in hertz, then `absoluteCents = 1200 * log2 (f/440) + 6900`. See also the AudioUnitParameterUnit.cents property.

## See Also

### Enumeration Cases

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

