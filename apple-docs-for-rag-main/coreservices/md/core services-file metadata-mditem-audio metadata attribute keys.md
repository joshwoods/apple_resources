

- Core Services
- File Metadata
- MDItem
-  Audio Metadata Attribute Keys 

API Collection

# Audio Metadata Attribute Keys

Metadata attribute keys that describe an audio file.

## Topics

### Constants

let kMDItemAppleLoopDescriptors: CFString!

Specifies multiple pieces of descriptive information about a loop. A CFArray of CFStrings.

let kMDItemAppleLoopsKeyFilterType: CFString!

Specifies key filtering information about a loop. Loops are matched against projects that often in a major or minor key. A CFString.

let kMDItemAppleLoopsLoopMode: CFString!

Specifies how a file should be played. A CFString.

let kMDItemAppleLoopsRootKey: CFString!

Specifies the loop's original key. The key is the root note or tonic for the loop, and does not include the scale type. A CFString.

let kMDItemAudioChannelCount: CFString!

Number of channels in the audio data contained in the file. A CFNumber.

let kMDItemAudioEncodingApplication: CFString!

The name of the application that encoded the data contained in the audio file. A CFString.

let kMDItemAudioSampleRate: CFString!

Sample rate of the audio data contained in the file. The sample rate is a float value representing hz (audio_frames/second). For example: 44100.0, 22254.54. A CFNumber.

let kMDItemAudioTrackNumber: CFString!

The track number of a song or composition when it is part of an album. A CFNumber (integer).

let kMDItemComposer: CFString!

The composer of the music contained in the audio file. A CFString.

let kMDItemIsGeneralMIDISequence: CFString!

Indicates whether the MIDI sequence contained in the file is setup for use with a General MIDI device. A CFBoolean.

let kMDItemKeySignature: CFString!

The key of the music contained in the audio file. For example: C, Dm, F#m, Bb. A CFString.

let kMDItemLyricist: CFString!

The lyricist, or text writer, of the music contained in the audio file. A CFString.

let kMDItemMusicalGenre: CFString!

The musical genre of the song or composition contained in the audio file. For example: Jazz, Pop, Rock, Classical. A CFString.

let kMDItemMusicalInstrumentCategory: CFString!

Specifies the category of an instrument. A CFString.

let kMDItemMusicalInstrumentName: CFString!

Specifies the name of instrument relative to the instrument category. A CFString.

let kMDItemRecordingDate: CFString!

The recording date of the song or composition.

let kMDItemRecordingYear: CFString!

Indicates the year the item was recorded. For example, 1964, 2003, etc. A CFNumber.

let kMDItemTempo: CFString!

A float value that specifies the beats per minute of the music contained in the audio file. A CFNumber.

let kMDItemTimeSignature: CFString!

The time signature of the musical composition contained in the audio/MIDI file. For example: "4/4", "7/8". A CFString.

