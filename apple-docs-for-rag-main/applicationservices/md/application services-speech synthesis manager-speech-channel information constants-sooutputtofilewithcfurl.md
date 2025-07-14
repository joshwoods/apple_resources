

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soOutputToFileWithCFURL 

Global Variable

# soOutputToFileWithCFURL

Pass a `CFURLRef` in the `speechInfo` parameter to write to this file, or `NULL` to generate sound.

macOS 10.3+

``` source
var soOutputToFileWithCFURL: OSType { get }
```

## Discussion

This selector works with the `SetSpeechInfo` function.

