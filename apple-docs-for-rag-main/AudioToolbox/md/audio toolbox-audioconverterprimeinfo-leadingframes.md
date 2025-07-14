

- Audio Toolbox
- AudioConverterPrimeInfo
-  leadingFrames 

Instance Property

# leadingFrames

The number of leading frames of input audio data required for the converter to perform high-quality conversion.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var leadingFrames: UInt32
```

## Discussion

This number is determined by the input audio format. Leading frames precede, in time, the desired starting input frame. If using the kConverterPrimeMethod_Pre value for the kAudioConverterPrimeMethod property, your application should provide the specified number of leading frames from the input stream when your input callback is first invoked. If no leading frames are available (because, for example, the desired start frame is at the very beginning of available audio), then your callback should provide the requested number of silent (`0`-valued) leading frames. Your callback should not provide a value for the leadingFrames field when the kAudioConverterPrimeMethod property value is kConverterPrimeMethod_Normal or kConverterPrimeMethod_None.

