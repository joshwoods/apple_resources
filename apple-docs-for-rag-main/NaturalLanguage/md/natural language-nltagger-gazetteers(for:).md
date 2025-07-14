

- Natural Language
- NLTagger
-  gazetteers(for:) 

Instance Method

# gazetteers(for:)

Retrieves the gazetteers attached to a tag scheme.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func gazetteers(for tagScheme: NLTagScheme) -> [NLGazetteer]
```

## Parameters 

`tagScheme`  

The tag scheme for the gazetteers.

## Return Value

An array of NLGazetteer.

## See Also

### Using gazetteers with a tagger

func setGazetteers([NLGazetteer], for: NLTagScheme)

Attaches gazetteers to a tag scheme, typically one gazetteer per language or one language-independent gazetteer.

class NLGazetteer

A collection of terms and their labels, which take precedence over a word tagger.

