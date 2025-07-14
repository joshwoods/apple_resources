

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechPitchModProperty 

Global Variable

# kSpeechPitchModProperty

Get or set a speech channel’s pitch modulation.

macOS 10.5+

``` source
let kSpeechPitchModProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object that specifies the speech channel’s pitch modulation.

Pitch modulation is also expressed as a floating-point value in the range of 0.000 to 127.000. These values correspond to MIDI note values, where 60.000 is equal to middle C on a piano scale. The most useful speech pitches fall in the range of 40.000 to 55.000. A pitch modulation value of 0.000 corresponds to a monotone in which all speech is generated at the frequency corresponding to the speech pitch. Given a speech pitch value of 46.000, a pitch modulation of 2.000 would mean that the widest possible range of pitches corresponding to the actual frequency of generated text would be 44.000 to 48.000.

This property works with the CopySpeechProperty(_:_:_:) and SetSpeechProperty(_:_:_:) functions.

Note

The change in pitch modulation may not be noticeable until the next sentence or paragraph is spoken.

