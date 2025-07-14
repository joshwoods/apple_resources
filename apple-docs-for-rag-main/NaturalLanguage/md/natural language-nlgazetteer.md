

- Natural Language
-  NLGazetteer 

Class

# NLGazetteer

A collection of terms and their labels, which take precedence over a word tagger.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NLGazetteer
```

## Overview

Use an NLGazetteer to augment an NLTagger when you need to tag a specific set of terms (single words or short phrases) with a label. Typically, you add one gazetteer per language, or one language-independent gazetteer, to an NLTagger with its setGazetteers(_:for:) method. The tagger uses its gazetteers to look up each term it processes. If a gazetteer has a label for a term, the tagger uses that label to tag the term, instead of inferring a tag itself.

Typically, you create a gazetteer at development time, such as in a macOS playground, with Create ML’s MLGazetteer. Alternatively, you can create an NLGazetteer at runtime by using init(dictionary:language:).

## Topics

### Creating a Gazetteer

init(contentsOf: URL) throws

Creates a Natural Language gazetteer from a model created with the Create ML framework.

init(data: Data) throws

Creates a gazetteer from a data instance.

init(dictionary: [String : [String]], language: NLLanguage?) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary.

class func write([String : [String]], language: NLLanguage?, to: URL) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary and saves the gazetteer to a file.

### Looking Up Labels for Terms

func label(for: String) -> String?

Retrieves the label for the given term.

### Inspecting a Gazetteer

var data: Data

The gazetteer represented as a data instance.

var language: NLLanguage?

The language of the gazetteer.

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

### Using gazetteers with a tagger

func setGazetteers([NLGazetteer], for: NLTagScheme)

Attaches gazetteers to a tag scheme, typically one gazetteer per language or one language-independent gazetteer.

func gazetteers(for: NLTagScheme) -> [NLGazetteer]

Retrieves the gazetteers attached to a tag scheme.

