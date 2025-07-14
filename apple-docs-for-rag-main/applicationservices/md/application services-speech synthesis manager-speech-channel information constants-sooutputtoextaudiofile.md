

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soOutputToExtAudioFile 

Global Variable

# soOutputToExtAudioFile

Pass an ExtAudioFileRef in the `speechInfo` parameter to write to this file, or `NULL` to generate sound.

macOS 10.6+

``` source
var soOutputToExtAudioFile: OSType { get }
```

## Discussion

Note that the Speech Synthesis Manager may alter the kExtAudioFileProperty_ClientDataFormat and kExtAudioFileProperty_ClientChannelLayout properties of the extended audio file object. The caller is responsible for closing the extended audio file object after the Speech Synthesis Manager is finished with it.

This selector works with the `SetSpeechInfo` function.

