

- Natural Language
- NLLanguageRecognizer
-  languageHypotheses(withMaximum:) 

Instance Method

# languageHypotheses(withMaximum:)

Generates the probabilities of possible languages for the processed text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func languageHypotheses(withMaximum maxHypotheses: Int) -> [NLLanguage : Double]
```

## Parameters 

`maxHypotheses`  

The maximum number of languages to return.

## Return Value

A dictionary mapping languages with their probabilities, up to `maxHypotheses` languages.

## See Also

### Determining the language

class func dominantLanguage(for: String) -> NLLanguage?

Finds the most likely language of a piece of text.

func processString(String)

Analyzes the piece of text to determine its dominant language.

var dominantLanguage: NLLanguage?

The most likely language for the processed text.

func reset()

Resets the recognizer to its initial state.

