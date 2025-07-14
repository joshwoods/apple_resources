

- Translation
- TranslationError
-  unsupportedLanguagePairing 

Type Property

# unsupportedLanguagePairing

The framework doesn’t support the the specified source and target language pairing.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
static let unsupportedLanguagePairing: TranslationError
```

## Discussion

The framework doesn’t support translating from and to the same language. For example you can’t translate from English (US) to English (UK) or from French to French.

## See Also

### Handling unsupported errors

static let unsupportedSourceLanguage: TranslationError

The framework doesn’t support the specified or detected source language.

static let unsupportedTargetLanguage: TranslationError

The framework doesn’t support the specified or chosen target language.

