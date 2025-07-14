

- AVFAudio
- AVAudioUnitSampler
-  loadSoundBankInstrument(at:program:bankMSB:bankLSB:) 

Instance Method

# loadSoundBankInstrument(at:program:bankMSB:bankLSB:)

Loads a specific instrument from the specified soundbank.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func loadSoundBankInstrument(
    at bankURL: URL,
    program: UInt8,
    bankMSB: UInt8,
    bankLSB: UInt8
) throws
```

## Parameters 

`bankURL`  

The URL for a soundbank file, either a DLS bank (`.dls`) or a SoundFont bank (`.sf2`).

`program`  

The program number for the instrument to load.

`bankMSB`  

The most significant bit for the bank number for the instrument to load. This is usually `0x79` for melodic instruments and `0x78` for percussion instruments.

`bankLSB`  

The least significant bit for the bank number for the instrument to load. This is often `0` and represents the bank variation.

## Discussion

Important

This method reads from the file and allocates memory. Don’t call it on a real-time thread.

## See Also

### Configuring the Sampler Audio Unit

func loadInstrument(at: URL) throws

Configures the sampler with the specified instrument file.

func loadAudioFiles(at: [URL]) throws

Configures the sampler by loading the specified audio files.

