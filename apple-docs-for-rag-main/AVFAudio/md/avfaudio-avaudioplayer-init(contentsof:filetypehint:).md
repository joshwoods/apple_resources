

- AVFAudio
- AVAudioPlayer
-  init(contentsOf:fileTypeHint:) 

Initializer

# init(contentsOf:fileTypeHint:)

Creates a player to play audio from a file of a particular type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    contentsOf url: URL,
    fileTypeHint utiString: String?
) throws
```

## Parameters 

`url`  

A URL that identifies the local audio file to play.

`utiString`  

The uniform type identifier (UTI) string of the file format.

## Return Value

A new audio player instance, or nil if there is an error.

## Discussion

The audio data must be in a format that Core Audio supports. Passing a file type hint helps the system parse the data if it can’t determine the file type or if the data is corrupt. See AVFileType for supported values.

## See Also

### Creating an audio player

init(contentsOf: URL) throws

Creates a player to play audio from a file.

init(data: Data) throws

Creates a player to play in-memory audio data.

init(data: Data, fileTypeHint: String?) throws

Creates a player to play in-memory audio data of a particular type.

