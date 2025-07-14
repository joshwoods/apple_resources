

- AVFAudio
- AVAudioUnitSampler
-  loadAudioFiles(at:) 

Instance Method

# loadAudioFiles(at:)

Configures the sampler by loading the specified audio files.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func loadAudioFiles(at audioFiles: [URL]) throws
```

## Parameters 

`audioFiles`  

An array of audio file URLs to load.

## Discussion

The framework loads the audio files into a new instrument with each audio file in its own sampler zone. The framework uses any information in the audio file for its placement in the instrument. For example, the root key and key range.

## See Also

### Configuring the Sampler Audio Unit

func loadInstrument(at: URL) throws

Configures the sampler with the specified instrument file.

func loadSoundBankInstrument(at: URL, program: UInt8, bankMSB: UInt8, bankLSB: UInt8) throws

Loads a specific instrument from the specified soundbank.

