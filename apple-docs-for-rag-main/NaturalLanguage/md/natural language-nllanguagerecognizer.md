

- Natural Language
-  NLLanguageRecognizer 

Class

# NLLanguageRecognizer

The language of a body of text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class NLLanguageRecognizer
```

## Mentioned in 

Identifying the language in text

## Overview

An NLLanguageRecognizer object automatically detects the language of a piece of text. It performs language identification by:

1.  Identifying the dominant script of a piece of text. Some languages have a unique script (like Greek), but others share the same script (like English, French, and German, which all share the Latin script).

2.  Identifying the language itself.

The identification obtained from an NLLanguageRecognizer object can be either a single most likely language, access through dominantLanguage, or a set of language candidates with probabilities, using languageHypothesesWithMaximum:. You can reset the recognizer to its initial state, to be reused for new analysis.

Use the convenience method, dominantLanguage(for:), to get the most likely language without creating an NLLanguageRecognizer.

Important

Don’t use an instance of NLLanguageRecognizer from more than one thread simultaneously.

## Topics

### Creating a recognizer

init()

Creates a recognizer that you can customize.

### Determining the language

class func dominantLanguage(for: String) -> NLLanguage?

Finds the most likely language of a piece of text.

func processString(String)

Analyzes the piece of text to determine its dominant language.

var dominantLanguage: NLLanguage?

The most likely language for the processed text.

func languageHypotheses(withMaximum: Int) -> [NLLanguage : Double]

Generates the probabilities of possible languages for the processed text.

func reset()

Resets the recognizer to its initial state.

### Guiding the recognizer

var languageHints: [NLLanguage : Double]

A dictionary that maps languages to their probabilities in the language identification process.

var languageConstraints: [NLLanguage]

Limits the set of possible languages that the recognizer will return.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Language identification

Identifying the language in text

Detect the language in a piece of text by using a language recognizer.

struct NLLanguage

The languages that the Natural Language framework supports.

