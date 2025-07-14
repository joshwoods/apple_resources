

- AVFAudio
- AVMIDIPlayer
-  init(contentsOf:soundBankURL:) 

Initializer

# init(contentsOf:soundBankURL:)

Creates a player to play a MIDI file with the specified soundbank.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(
    contentsOf inURL: URL,
    soundBankURL bankURL: URL?
) throws
```

## Parameters 

`inURL`  

The URL of the file to play.

`bankURL`  

The URL of the sound bank. The sound bank must be in SoundFont2 or DLS format. In macOS, you can pass nil for the bank URL argument to use the default sound bank. In iOS, you must always pass a valid bank file.

## Return Value

A new MIDI player, or nil if an error occurred.

## See Also

### Creating a MIDI player

init(data: Data, soundBankURL: URL?) throws

Creates a player to play MIDI data with the specified soundbank.

