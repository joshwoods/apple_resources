

- Application Services
- Speech Synthesis Manager
- VoiceFileInfo
-  fileSpec 

Instance Property

# fileSpec

A file system specification structure that contains the volume, directory, and name of the file containing the voice. Generally, files containing a single voice are of type `kTextToSpeechVoiceFileType`, and files containing multiple voices are of type `kTextToSpeechVoiceBundleType`.

macOS 10.0+

``` source
var fileSpec: FSSpec
```

