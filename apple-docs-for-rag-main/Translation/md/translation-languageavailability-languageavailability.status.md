

- Translation
- LanguageAvailability
-  LanguageAvailability.Status 

Enumeration

# LanguageAvailability.Status

The availability status for a language or language pairing.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
enum Status
```

## Overview

A language must download and install before you can use it in a translation.

## Topics

### Operators

static func == (LanguageAvailability.Status, LanguageAvailability.Status) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case installed

A language or language pairing the framework supports, has downloaded and made ready for use in a translation.

case supported

A language or language pairing the framework supports but can’t yet use.

case unsupported

A language or language pairing the framework doesn’t support.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Checking availability

func status(from: Locale.Language, to: Locale.Language?) async -> LanguageAvailability.Status

Checks to see if a specific language pairing is installed and ready for translation.

func status(for: String, to: Locale.Language?) async throws -> LanguageAvailability.Status

Checks to see if a language pairing is supported based off a string of sample text.

