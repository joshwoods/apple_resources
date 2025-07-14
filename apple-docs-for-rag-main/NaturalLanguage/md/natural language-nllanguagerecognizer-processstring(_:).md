

- Natural Language
- NLLanguageRecognizer
-  processString(\_:) 

Instance Method

# processString(\_:)

Analyzes the piece of text to determine its dominant language.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func processString(_ string: String)
```

## Mentioned in 

Identifying the language in text

## Discussion

Use this method to process the provided text and to update the dominantLanguage result and `languageHypotheses(withMaximum:)` probabilities.

## See Also

### Determining the language

class func dominantLanguage(for: String) -> NLLanguage?

Finds the most likely language of a piece of text.

var dominantLanguage: NLLanguage?

The most likely language for the processed text.

func languageHypotheses(withMaximum: Int) -> [NLLanguage : Double]

Generates the probabilities of possible languages for the processed text.

func reset()

Resets the recognizer to its initial state.

