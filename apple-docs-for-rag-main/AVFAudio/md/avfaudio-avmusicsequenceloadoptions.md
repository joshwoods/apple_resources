

- AVFAudio
-  AVMusicSequenceLoadOptions 

Structure

# AVMusicSequenceLoadOptions

A structure that defines whether data on different MIDI channels map to multiple tracks, or whether the framework preserves the tracks as they are.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMusicSequenceLoadOptions
```

## Topics

### Getting Standard Load Options

static var smf_ChannelsToTracks: AVMusicSequenceLoadOptions

An option that represents data on different MIDI channels mapped to multiple tracks.

### Creating a Load Option

init(rawValue: UInt)

Creates a new instance with the raw value you specify.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Managing Sequence Load Options

func load(from: Data, options: AVMusicSequenceLoadOptions) throws

Parses the data and adds its events to the sequence.

func load(from: URL, options: AVMusicSequenceLoadOptions) throws

Loads the file the URL references and adds the events to the sequence.

