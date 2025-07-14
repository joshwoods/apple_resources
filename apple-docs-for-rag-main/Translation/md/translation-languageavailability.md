

- Translation
-  LanguageAvailability 

Class

# LanguageAvailability

A check for language support and status.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
class LanguageAvailability
```

## Overview

Use this class to check and see whether the framework supports the language or language pairing you want to offer as a translation. For example, to check if someone’s device supports a translation you can do the following:

```
```

## Topics

### Creating a language availability

init()

Creates a language availability.

### Getting supported languages

var supportedLanguages: [Locale.Language]

A list of translation languages the framework supports.

### Checking availability

func status(from: Locale.Language, to: Locale.Language?) async -> LanguageAvailability.Status

Checks to see if a specific language pairing is installed and ready for translation.

func status(for: String, to: Locale.Language?) async throws -> LanguageAvailability.Status

Checks to see if a language pairing is supported based off a string of sample text.

enum Status

The availability status for a language or language pairing.

