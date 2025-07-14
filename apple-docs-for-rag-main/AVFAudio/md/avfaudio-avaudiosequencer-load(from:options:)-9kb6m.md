

- AVFAudio
- AVAudioSequencer
-  load(from:options:) 

Instance Method

# load(from:options:)

Loads the file the URL references and adds the events to the sequence.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func load(
    from fileURL: URL,
    options: AVMusicSequenceLoadOptions = []
) throws
```

## Parameters 

`fileURL`  

The URL to the file.

`options`  

Determines how the contents map to the tracks inside the sequence.

## See Also

### Managing Sequence Load Options

func load(from: Data, options: AVMusicSequenceLoadOptions) throws

Parses the data and adds its events to the sequence.

struct AVMusicSequenceLoadOptions

A structure that defines whether data on different MIDI channels map to multiple tracks, or whether the framework preserves the tracks as they are.

