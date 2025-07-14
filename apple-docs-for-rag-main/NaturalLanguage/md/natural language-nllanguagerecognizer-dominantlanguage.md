

- Natural Language
- NLLanguageRecognizer
-  dominantLanguage 

Instance Property

# dominantLanguage

The most likely language for the processed text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var dominantLanguage: NLLanguage? { get }
```

## Mentioned in 

Identifying the language in text

## See Also

### Determining the language

class func dominantLanguage(for: String) -> NLLanguage?

Finds the most likely language of a piece of text.

func processString(String)

Analyzes the piece of text to determine its dominant language.

func languageHypotheses(withMaximum: Int) -> [NLLanguage : Double]

Generates the probabilities of possible languages for the processed text.

func reset()

Resets the recognizer to its initial state.

