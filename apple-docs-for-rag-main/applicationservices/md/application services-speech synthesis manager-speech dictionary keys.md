

- Application Services
- Speech Synthesis Manager
-  Speech Dictionary Keys 

API Collection

# Speech Dictionary Keys

Keys used in a speech dictionary to override the synthesizer’s default pronunciation of a word.

## Overview

The keys in a speech dictionary can determine how a synthesizer pronounces a word. After you’ve created a speech dictionary, you register it with a speech channel with the UseSpeechDictionary(_:_:) function.

## Topics

### Constants

let kSpeechDictionaryLocaleIdentifier: CFString

The locale associated with the pronunciation.

let kSpeechDictionaryModificationDate: CFString

The date the dictionary was last modified.

let kSpeechDictionaryPronunciations: CFString

The set of custom pronunciations.

let kSpeechDictionaryAbbreviations: CFString

The set of custom pronunciations for abbreviations.

let kSpeechDictionaryEntrySpelling: CFString

The spelling of an entry.

let kSpeechDictionaryEntryPhonemes: CFString

The phonemic representation of an entry.

