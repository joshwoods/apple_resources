

- AVFAudio
-  AVSpeechSynthesisProviderVoice 

Class

# AVSpeechSynthesisProviderVoice

An object that represents a voice that an audio unit provides to its host.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class AVSpeechSynthesisProviderVoice
```

## Overview

This is a voice that an AVSpeechSynthesisProviderAudioUnit provides to the system, distinct from AVSpeechSynthesisVoice. Use speechVoices to access the underlying AVSpeechSynthesisVoice in the voice quality AVSpeechSynthesisVoiceQuality.enhanced.

## Topics

### Creating a voice

init(name: String, identifier: String, primaryLanguages: [String], supportedLanguages: [String])

Creates a voice with a name, an identifier, and language information.

### Inspecting a voice

var age: Int

The age of the voice, in years.

var gender: AVSpeechSynthesisVoiceGender

The gender of the voice.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

var identifier: String

The unique identifier for the voice.

var name: String

The localized name of the voice.

var primaryLanguages: [String]

A list of BCP 47 codes that identify the languages the synthesizer uses.

var supportedLanguages: [String]

A list of BCP 47 codes that identify the languages a voice supports.

var version: String

The version of the voice.

var voiceSize: Int64

The size of the voice package on disk, in bytes.

### Updating a voice

class func updateSpeechVoices()

Updates the voices your app provides to the system.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Getting and setting voices

var speechVoices: [AVSpeechSynthesisProviderVoice]

A list of voices the audio unit provides to the system.

