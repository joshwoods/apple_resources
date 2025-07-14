

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soPhonemeSymbols 

Global Variable

# soPhonemeSymbols

macOS 10.0+

``` source
var soPhonemeSymbols: OSType { get }
```

## Discussion

Get a list of phoneme symbols and example wordsdefined for the speech channel’s synthesizer. Your applicationmight use this information to show the user what symbols to usewhen entering phonemic text directly. The `speechInfo` parameteris a pointer to a variable of type Handle that, on exit from the `GetSpeechInfo` function,is a handle to a phoneme descriptor structure, described in PhonemeDescriptor.

This selector works with the `GetSpeechInfo` function.

