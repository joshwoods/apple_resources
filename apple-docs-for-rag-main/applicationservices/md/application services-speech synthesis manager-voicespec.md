

- Application Services
- Speech Synthesis Manager
-  VoiceSpec 

Structure

# VoiceSpec

Defines a voice specification structure.

macOS 10.0+

``` source
struct VoiceSpec
```

## Overview

A voice specification structure provides a unique specification that you must use to obtain information about a voice. You also must use a voice specification structure if you wish to create a speech channel that generates speech in a voice other than the current system default voice.

To ensure compatibility with future versions of the Speech Synthesis Manager, you should never fill in the fields of a voice specification structure yourself. Instead, you should create a voice specification structure by using the MakeVoiceSpec(_:_:_:) function.

## Topics

### Initializers

init()

init(creator: OSType, id: OSType)

### Instance Properties

var creator: OSType

The synthesizer that is required to use the voice. This is equivalent to the value contained in the `synthManufacturer` field of a speech version information structure and that contained in the `synthCreator` field of a speech extension data structure. The set of `OSType` values specified entirely by space characters and lowercase letters is reserved.

var id: OSType

The voice ID of the voice for the synthesizer. Every voice on a synthesizer has a unique ID.

