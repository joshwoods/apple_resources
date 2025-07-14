

- AVFAudio
-  AVSpeechSynthesisVoice 

Class

# AVSpeechSynthesisVoice

A distinct voice for use in speech synthesis.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class AVSpeechSynthesisVoice
```

## Overview

The primary factors that distinguish a voice in speech synthesis are language, locale, and quality. Create an instance of `AVSpeechSynthesisVoice` to select a voice that’s appropriate for the text and the language, and set it as the value of the voice property on an AVSpeechUtterance instance. The voice may optionally reflect a local variant of the language, such as Australian or South African English. For a complete list of supported languages, see Languages Supported by VoiceOver.

## Topics

### Obtaining voices

init?(identifier: String)

Retrieves a voice for the identifier you specify.

init?(language: String?)

Retrieves a voice for the BCP 47 code language code you specify.

class func speechVoices() -> [AVSpeechSynthesisVoice]

Retrieves all available voices on the device.

let AVSpeechSynthesisVoiceIdentifierAlex: String

The voice that the system identifies as Alex.

### Inspecting voices

var identifier: String

The unique identifier of a voice.

var name: String

The name of a voice.

var quality: AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

var gender: AVSpeechSynthesisVoiceGender

The gender for a voice.

var voiceTraits: AVSpeechSynthesisVoice.Traits

The traits of a voice.

var audioFileSettings: [String : Any]

A dictionary that contains audio file settings.

enum AVSpeechSynthesisVoiceQuality

The speech quality of a voice.

enum AVSpeechSynthesisVoiceGender

The gender for a voice.

struct Traits

Traits that describe a voice.

### Working with language codes

class func currentLanguageCode() -> String

Returns the language and locale code for the user’s current locale.

var language: String

A BCP 47 code that contains the voice’s language and locale.

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
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Spoken text attributes

class AVSpeechUtterance

An object that encapsulates the text for speech synthesis and parameters that affect the speech.

