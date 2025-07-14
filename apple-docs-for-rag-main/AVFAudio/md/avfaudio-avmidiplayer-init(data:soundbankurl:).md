

- AVFAudio
- AVMIDIPlayer
-  init(data:soundBankURL:) 

Initializer

# init(data:soundBankURL:)

Creates a player to play MIDI data with the specified soundbank.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(
    data: Data,
    soundBankURL bankURL: URL?
) throws
```

## Parameters 

`data`  

The data to play.

`bankURL`  

The URL of the sound bank. The sound bank must be a SoundFont2 or DLS bank. In macOS, you can pass nil for the bank URL argument to use the default sound bank. In iOS, you must always pass a valid bank file.

## Return Value

A new MIDI player, or nil if an error occurred.

## See Also

### Creating a MIDI player

init(contentsOf: URL, soundBankURL: URL?) throws

Creates a player to play a MIDI file with the specified soundbank.

