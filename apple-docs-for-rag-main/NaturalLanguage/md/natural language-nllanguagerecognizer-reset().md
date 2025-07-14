

- Natural Language
- NLLanguageRecognizer
-  reset() 

Instance Method

# reset()

Resets the recognizer to its initial state.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func reset()
```

## See Also

### Determining the language

class func dominantLanguage(for: String) -> NLLanguage?

Finds the most likely language of a piece of text.

func processString(String)

Analyzes the piece of text to determine its dominant language.

var dominantLanguage: NLLanguage?

The most likely language for the processed text.

func languageHypotheses(withMaximum: Int) -> [NLLanguage : Double]

Generates the probabilities of possible languages for the processed text.

