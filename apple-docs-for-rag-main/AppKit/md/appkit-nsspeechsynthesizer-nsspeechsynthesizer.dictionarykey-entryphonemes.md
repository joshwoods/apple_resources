

- AppKit
- NSSpeechSynthesizer
- NSSpeechSynthesizer.DictionaryKey
-  entryPhonemes 

Type Property

# entryPhonemes

The phonemic representation of an entry. An `NSString`.

macOS 10.5+

``` source
static let entryPhonemes: NSSpeechSynthesizer.DictionaryKey
```

## See Also

### Type Properties

static let abbreviations: NSSpeechSynthesizer.DictionaryKey

An array of dictionary objects containing the keys entrySpelling and entryPhonemes.

static let entrySpelling: NSSpeechSynthesizer.DictionaryKey

The spelling of an entry. An `NSString`.

static let localeIdentifier: NSSpeechSynthesizer.DictionaryKey

The canonical locale identifier string describing the dictionary’s locale. A locale is generally composed of three pieces of ordered information: a language code, a region code, and a variant code. Refer to documentation about NSLocale or Internationalization and Localization Guide for more information

static let modificationDate: NSSpeechSynthesizer.DictionaryKey

A string representation of the dictionary’s last modification date in the international format (YYYY-MM-DD HH:MM:SS ±HHMM). If the same word appears across multiple dictionaries, the one from the dictionary with the most recent date will be used.

static let pronunciations: NSSpeechSynthesizer.DictionaryKey

An array of dictionary objects containing the keys entrySpelling and entryPhonemes.

