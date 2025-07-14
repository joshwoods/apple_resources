

- Application Services
- Speech Synthesis Manager
-  SpeechVersionInfo 

Structure

# SpeechVersionInfo

Defines a speech version information structure.

macOS 10.0+

``` source
struct SpeechVersionInfo
```

## Overview

By calling the GetSpeechInfo function with the `soSynthType` selector, you can obtain a speech version information structure, which provides information about the speech synthesizer currently being used.

## Topics

### Initializers

init()

init(synthType: OSType, synthSubType: OSType, synthManufacturer: OSType, synthFlags: Int32, synthVersion: NumVersion)

### Instance Properties

var synthFlags: Int32

A set of flags indicating which synthesizer features are activated. Specific constants define the bits in this field whose meanings are defined for all synthesizers.

var synthManufacturer: OSType

A unique identification of a synthesizer engine. If you develop synthesizers, then you should register a different four-character code for each synthesizer you develop with Developer Technical Support. The `creatorID` field of the voice specification structure and the `synthCreator` field of a speech extension data structure should each be set to the value stored in this field for the desired synthesizer.

var synthSubType: OSType

The specific type of the synthesizer. Currently, no specific types of synthesizer are defined. If you define a new type of synthesizer, you should register the four-character code for your type with Developer Technical Support.

var synthType: OSType

The general type of the synthesizer. For the current version of the Speech Synthesis Manager, this field always contains the value `kTextToSpeechSynthType`, indicating that the synthesizer converts text into speech.

var synthVersion: NumVersion

The version number of the synthesizer.

