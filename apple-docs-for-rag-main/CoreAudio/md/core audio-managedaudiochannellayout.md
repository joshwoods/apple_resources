

- Core Audio
-  ManagedAudioChannelLayout 

Structure

# ManagedAudioChannelLayout

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
struct ManagedAudioChannelLayout
```

## Topics

### Structures

struct ChannelDescriptions

### Initializers

init(audioChannelLayoutPointer: AudioChannelLayout.UnsafePointer, deallocator: (AudioChannelLayout.UnsafePointer) -> Void)

init(channelDescriptions: [AudioChannelDescription])

init(maximumDescriptions: Int)

init(tag: AudioChannelLayoutTag)

### Instance Properties

var bitmap: AudioChannelBitmap

var channelDescriptions: ManagedAudioChannelLayout.ChannelDescriptions

var numberOfChannels: Int

var sizeInBytes: Int

var tag: AudioChannelLayoutTag

### Instance Methods

func setAllToUnknown()

func withUnsafeMutablePointer&lt;Result>((UnsafeMutablePointer&lt;AudioChannelLayout>) throws -> Result) rethrows -> Result

func withUnsafePointer&lt;Result>((UnsafePointer&lt;AudioChannelLayout>) throws -> Result) rethrows -> Result

## Relationships

### Conforms To

- Copyable
- Equatable

