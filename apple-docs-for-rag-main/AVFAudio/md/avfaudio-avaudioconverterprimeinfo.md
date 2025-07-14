

- AVFAudio
-  AVAudioConverterPrimeInfo 

Structure

# AVAudioConverterPrimeInfo

Priming information for audio conversion.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAudioConverterPrimeInfo
```

## Topics

### Creating Priming Information

init()

Creates a priming information instance.

init(leadingFrames: AVAudioFrameCount, trailingFrames: AVAudioFrameCount)

Creates a priming information instance with the specified leading and trailing frames.

### Getting Frame Properties

var leadingFrames: AVAudioFrameCount

The number of leading (previous) input frames the converter requires to perform a high-quality conversion.

var trailingFrames: AVAudioFrameCount

The number of trailing input frames, past the end input frame, the converter requires to perform a high-quality conversion.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting Priming Information

var primeInfo: AVAudioConverterPrimeInfo

The number of priming frames the converter uses.

var primeMethod: AVAudioConverterPrimeMethod

The priming method the sample rate converter or decoder uses.

enum AVAudioConverterPrimeMethod

Options for the prime method property.

