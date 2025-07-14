

- Application Services
- Speech Synthesis Manager
-  VoiceFileInfo 

Structure

# VoiceFileInfo

Defines a voice file information structure.

macOS 10.0+

``` source
struct VoiceFileInfo
```

## Overview

A voice file information structure specifies the file in which a voice is stored and the resource ID of the voice within that file. Use the GetVoiceInfo(_:_:_:) function to obtain a voice file information structure for a voice.

## Topics

### Initializers

init()

init(fileSpec: FSSpec, resID: Int16)

### Instance Properties

var fileSpec: FSSpec

A file system specification structure that contains the volume, directory, and name of the file containing the voice. Generally, files containing a single voice are of type `kTextToSpeechVoiceFileType`, and files containing multiple voices are of type `kTextToSpeechVoiceBundleType`.

var resID: Int16

The resource ID of the voice in the file. Voices are stored in resources of type `kTextToSpeechVoiceType`.

