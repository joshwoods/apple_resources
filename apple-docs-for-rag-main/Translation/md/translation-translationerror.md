

- Translation
-  TranslationError 

Structure

# TranslationError

Error codes describing why the framework can’t perform a translation.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
struct TranslationError
```

## Topics

### Handling general errors

static let nothingToTranslate: TranslationError

No content to translate.

static let unableToIdentifyLanguage: TranslationError

The framework can’t identify the source language automatically.

static let internalError: TranslationError

An error occurred internal to the translation engine.

### Handling unsupported errors

static let unsupportedSourceLanguage: TranslationError

The framework doesn’t support the specified or detected source language.

static let unsupportedTargetLanguage: TranslationError

The framework doesn’t support the specified or chosen target language.

static let unsupportedLanguagePairing: TranslationError

The framework doesn’t support the the specified source and target language pairing.

### Operators

static func ~= (TranslationError, any Error) -> Bool

You can use `switch` and `case` to check for a given value of `TranslationError` if you want to handle each error case separately.

### Instance Properties

var errorDescription: String?

A localized message describing what error occurred.

var failureReason: String?

A localized message describing the reason for the failure.

### Default Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Error
- LocalizedError
- Sendable

