

- Natural Language
- NLLanguageRecognizer
-  dominantLanguage(for:) 

Type Method

# dominantLanguage(for:)

Finds the most likely language of a piece of text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class func dominantLanguage(for string: String) -> NLLanguage?
```

## Parameters 

`string`  

The text to analyze.

## Return Value

The most probable language of the piece of text.

## See Also

### Determining the language

func processString(String)

Analyzes the piece of text to determine its dominant language.

var dominantLanguage: NLLanguage?

The most likely language for the processed text.

func languageHypotheses(withMaximum: Int) -> [NLLanguage : Double]

Generates the probabilities of possible languages for the processed text.

func reset()

Resets the recognizer to its initial state.

