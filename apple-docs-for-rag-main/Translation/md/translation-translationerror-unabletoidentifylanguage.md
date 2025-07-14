

- Translation
- TranslationError
-  unableToIdentifyLanguage 

Type Property

# unableToIdentifyLanguage

The framework can’t identify the source language automatically.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
static let unableToIdentifyLanguage: TranslationError
```

## Discussion

This error is thrown when you call prepareTranslation() without specifying the source language, or when using status(for:to:) and the system can’t automatically identify the source language of the sample text you pass in.

Note

For best results in automatic language detection, pass in a sample string of at least 20 characters in length.

## See Also

### Handling general errors

static let nothingToTranslate: TranslationError

No content to translate.

static let internalError: TranslationError

An error occurred internal to the translation engine.

