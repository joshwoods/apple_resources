

- Audio Toolbox
- MusicSequenceType
-  MusicSequenceType.seconds 

Case

# MusicSequenceType.seconds

Used for a music sequence that corresponds to a MIDI file, but employs SMPTE timecode. The tempo track contains a single tempo event that specifies 60 beat-per-minute.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
case seconds
```

## See Also

### Constants

case beats

Used for a music sequence that corresponds to a normal MIDI file. The tempo track defines the number of beats per second and can have multiple tempo events.

case samples

Used for audio samples; a music sequence of this type cannot be saved to a MIDI file. The tempo track contains a single tempo event that specifies an audio sample rate in samples-per-second.

