

- AVFAudio
- AVAudioPlayer
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates a player to play audio from a file.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
init(contentsOf url: URL) throws
```

## Parameters 

`url`  

A URL that identifies the local audio file to play.

## Return Value

A new audio player instance, or nil if an error occurs.

## Discussion

The audio data must be in a format that Core Audio supports.

## See Also

### Creating an audio player

init(contentsOf: URL, fileTypeHint: String?) throws

Creates a player to play audio from a file of a particular type.

init(data: Data) throws

Creates a player to play in-memory audio data.

init(data: Data, fileTypeHint: String?) throws

Creates a player to play in-memory audio data of a particular type.

