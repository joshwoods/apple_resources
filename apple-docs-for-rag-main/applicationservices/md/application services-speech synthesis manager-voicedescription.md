

- Application Services
- Speech Synthesis Manager
-  VoiceDescription 

Structure

# VoiceDescription

Defines a voice description structure.

macOS 10.0+

``` source
struct VoiceDescription
```

## Overview

By calling the GetVoiceDescription(_:_:_:) function, you can obtain information about a voice in a voice description structure.

## Topics

### Initializers

init()

init(length: Int32, voice: VoiceSpec, version: Int32, name: Str63, comment: Str255, gender: Int16, age: Int16, script: Int16, language: Int16, region: Int16, reserved: (Int32, Int32, Int32, Int32))

### Instance Properties

var age: Int16

The approximate age in years of the individual represented by the voice.

var comment: Str255

Additional text information about the voice. Some synthesizers use this field to store a phrase that can be spoken.

var gender: Int16

The gender of the individual represented by the voice. See Gender Constants.

var language: Int16

A code that indicates the language of voice output.

var length: Int32

The size of the voice description structure, in bytes.

var name: Str63

The name of the voice, preceded by a length byte. Names must be 63 characters or less.

var region: Int16

A code that indicates the region represented by the voice.

var reserved: (Int32, Int32, Int32, Int32)

Reserved. May be used to hold a 32-bit encoding value, if necessary (see the description of the `script` field for more information).

var script: Int16

The encoding code of the text that the voice can process.

var version: Int32

The version number of the voice.

var voice: VoiceSpec

A voice specification structure that uniquely identifies the voice.

