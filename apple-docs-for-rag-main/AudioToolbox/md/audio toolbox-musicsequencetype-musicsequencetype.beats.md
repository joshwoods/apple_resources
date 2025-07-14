

- Audio Toolbox
- MusicSequenceType
-  MusicSequenceType.beats 

Case

# MusicSequenceType.beats

Used for a music sequence that corresponds to a normal MIDI file. The tempo track defines the number of beats per second and can have multiple tempo events.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case beats
```

## See Also

### Constants

case seconds

Used for a music sequence that corresponds to a MIDI file, but employs SMPTE timecode. The tempo track contains a single tempo event that specifies 60 beat-per-minute.

case samples

Used for audio samples; a music sequence of this type cannot be saved to a MIDI file. The tempo track contains a single tempo event that specifies an audio sample rate in samples-per-second.

