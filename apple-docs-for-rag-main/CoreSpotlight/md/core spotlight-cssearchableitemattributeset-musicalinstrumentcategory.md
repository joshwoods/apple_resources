

- Core Spotlight
- CSSearchableItemAttributeSet
-  musicalInstrumentCategory 

Instance Property

# musicalInstrumentCategory

The category of the instrument associated with the audio file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var musicalInstrumentCategory: String? { get set }
```

## Discussion

A file should specify an associated instrument (note that you can use “Other Instrument” to specify an unknown instrument). In some categories, you can use instrument names to provide a more detailed instrument definition. For example, the Keyboards category lets you include instrument names such as Piano or Organ.

## See Also

### Describing music

var album: String?

The title for a collection of audio media.

var artist: String?

The artist associated with the media.

var audioChannelCount: NSNumber?

The number of channels in the audio data that the file contains.

var audioEncodingApplication: String?

The name of the application that encoded the data the audio file contains.

var audioSampleRate: NSNumber?

The sample rate of the audio data the file contains, as a float value representing Hz (audio frames per second), such as 44100.0 or 22254.54.

var audioTrackNumber: NSNumber?

The track number of a song or audio composition when part of an album.

var composer: String?

The composer of the song or audio composition that the audio file contains.

var keySignature: String?

The musical key of the song or audio composition that the file contains, such as C, Dm, or F#m.

var lyricist: String?

The lyricist or text writer for the song or audio composition that the file contains.

var musicalGenre: String?

The musical genre of the song or audio composition that the file contains, such as jazz, pop, rock, or classical.

var recordingDate: Date?

The recording date of the song or composition.

var tempo: NSNumber?

The tempo of the music that the audio file contains, in beats per minute.

var timeSignature: String?

The time signature of the musical composition that the audio or MIDI file contains, in a string, such as “4/4” or “7/8”.

var generalMIDISequence: NSNumber?

A value that indicates whether the MIDI sequence the file contains is set up for use with a general MIDI device.

var musicalInstrumentName: String?

The name of an instrument within the context of an instrument category.

