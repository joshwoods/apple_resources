

- Natural Language
- NLLanguageRecognizer
-  languageHints 

Instance Property

# languageHints

A dictionary that maps languages to their probabilities in the language identification process.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
var languageHints: [NLLanguage : Double] { get set }
```

## Discussion

This is a dictionary mapping languages to their probabilities and used by processString(_:).

## See Also

### Guiding the recognizer

var languageConstraints: [NLLanguage]

Limits the set of possible languages that the recognizer will return.

