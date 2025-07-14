

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soRate 

Global Variable

# soRate

macOS 10.0+

``` source
var soRate: OSType { get }
```

## Discussion

Get or set a speech channel’s speech rate.The `speechInfo` parameteris a pointer to a variable of type `Fixed`.The possible range of speech rates is from 0.000 to 65535.65535.The range of supported rates is not predefined by the Speech SynthesisManager; each speech synthesizer provides its own range of speechrates. Average human speech occurs at a rate of 180 to 220 words perminute.

This selector works with both the `GetSpeechInfo` and `SetSpeechInfo` functions.

