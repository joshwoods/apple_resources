

- Translation
- LanguageAvailability
-  status(for:to:) 

Instance Method

# status(for:to:)

Checks to see if a language pairing is supported based off a string of sample text.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
func status(
    for text: String,
    to target: Locale.Language?
) async throws -> LanguageAvailability.Status
```

## Parameters 

`text`  

A sample string of text representing the source language you want to translation from.

`target`  

The target language you want to translate content into. When set to `nil` the system picks an appropriate target based on the user’s preferred languages and returns the status for those languages.

## Return Value

The availability status for the language pairing to use in the translation.

## Discussion

Use this function when you don’t know the source language and you want the framework to attempt a translation for you based on the sample text you pass in.

Pass in a string of sample `text` representing the language you want to translate from. When you do, the system automatically tries to detect the language of the text you pass in. If it can’t, it throws a TranslationError.

If it can detect the source language of the text, it checks to see if the necessary language assets have downloaded and are ready for use.

Note

For best results in automatic language detection, pass in a sample string of at least 20 characters in length.

## See Also

### Checking availability

func status(from: Locale.Language, to: Locale.Language?) async -> LanguageAvailability.Status

Checks to see if a specific language pairing is installed and ready for translation.

enum Status

The availability status for a language or language pairing.

