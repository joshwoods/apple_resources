

- AVFAudio
- AVAudioPlayer
-  init(data:) 

Initializer

# init(data:)

Creates a player to play in-memory audio data.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
init(data: Data) throws
```

## Parameters 

`data`  

A buffer with the audio data to play.

## Return Value

A new audio player instance, or nil if an error occurs.

## Discussion

The audio data must be in a format that Core Audio supports.

## See Also

### Creating an audio player

init(contentsOf: URL) throws

Creates a player to play audio from a file.

init(contentsOf: URL, fileTypeHint: String?) throws

Creates a player to play audio from a file of a particular type.

init(data: Data, fileTypeHint: String?) throws

Creates a player to play in-memory audio data of a particular type.

