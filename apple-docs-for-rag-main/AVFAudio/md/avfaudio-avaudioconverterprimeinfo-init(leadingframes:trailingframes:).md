

- AVFAudio
- AVAudioConverterPrimeInfo
-  init(leadingFrames:trailingFrames:) 

Initializer

# init(leadingFrames:trailingFrames:)

Creates a priming information instance with the specified leading and trailing frames.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    leadingFrames: AVAudioFrameCount,
    trailingFrames: AVAudioFrameCount
)
```

## Parameters 

`leadingFrames`  

Specifies the number of leading (previous) input frames relative to the start input frame.

`trailingFrames`  

Specifies the number of trailing input frames past the end input frame.

## See Also

### Creating Priming Information

init()

Creates a priming information instance.

