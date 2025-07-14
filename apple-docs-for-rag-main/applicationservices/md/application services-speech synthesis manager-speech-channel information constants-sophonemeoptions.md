

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soPhonemeOptions 

Global Variable

# soPhonemeOptions

Get or set options for the generation of phonetic output. See Phoneme Generation Options for a complete list of options.

macOS 10.6+

``` source
var soPhonemeOptions: OSType { get }
```

## Discussion

The `speechInfo` parameter is a pointer to a long value that represents the phoneme generation value.

This selector works with both the `GetSpeechInfo` and `SetSpeechInfo` functions.

