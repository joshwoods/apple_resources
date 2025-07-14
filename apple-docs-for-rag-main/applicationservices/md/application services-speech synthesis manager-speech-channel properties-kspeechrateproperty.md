

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechRateProperty 

Global Variable

# kSpeechRateProperty

Get or set a speech channel’s speech rate.

macOS 10.5+

``` source
let kSpeechRateProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object that specifies the speech channel’s speaking rate.

The range of supported rates is not predefined by the Speech Synthesis Manager; each speech synthesizer provides its own range of speech rates. Average human speech occurs at a rate of 180 to 220 words per minute.

This property works with the CopySpeechProperty(_:_:_:) and SetSpeechProperty(_:_:_:) functions.

