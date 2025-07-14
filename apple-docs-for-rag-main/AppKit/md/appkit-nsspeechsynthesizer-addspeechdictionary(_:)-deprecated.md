

- AppKit
- NSSpeechSynthesizer
-  addSpeechDictionary(\_:) Deprecated

Instance Method

# addSpeechDictionary(\_:)

Registers the given speech dictionary with the receiver.

macOS 10.5–14.0Deprecated

``` source
func addSpeechDictionary(_ speechDictionary: [NSSpeechSynthesizer.DictionaryKey : Any])
```

## Parameters 

`speechDictionary`  

Speech dictionary to add to the receiver’s dictionaries. The key-value pairs are listed in `Speech Dictionary Properties Keys`.

## Discussion

See the discussion of UseSpeechDictionary(_:_:) in Speech Synthesis Manager for more information.

## See Also

### Configuring Speech Attributes

struct DictionaryKey

These constants identify key-value pairs used to add vocabulary to the dictionary using addSpeechDictionary(_:).

Deprecated

func object(forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws -> Any

Provides the value of a receiver’s property.

Deprecated

func setObject(Any?, forProperty: NSSpeechSynthesizer.SpeechPropertyKey) throws

Specifies the value of a receiver’s property.

Deprecated

struct SpeechPropertyKey

These constants are used with setObject(_:forProperty:) and object(forProperty:) to get or set the characteristics of a synthesizer.

Deprecated

struct CommandDelimiterKey

Keys for the command delimiters.

Deprecated

struct ErrorKey

Keys that identify errors that may occur during speech synthesis.

Deprecated

struct Mode

Keys for the speaking mode.

Deprecated

struct PhonemeInfoKey

Keys for the speech phoneme information.

Deprecated

struct StatusKey

Keys for the speech synthesizier status.

Deprecated

struct SynthesizerInfoKey

Keys for the speech synthesizier information.

Deprecated

struct VoiceGender

The following constants define voice gender attributes, which are the allowable values of the gender key returned by attributes(forVoice:).

Deprecated

