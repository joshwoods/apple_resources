

- Natural Language
- NLTagger
-  setGazetteers(\_:for:) 

Instance Method

# setGazetteers(\_:for:)

Attaches gazetteers to a tag scheme, typically one gazetteer per language or one language-independent gazetteer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setGazetteers(
    _ gazetteers: [NLGazetteer],
    for tagScheme: NLTagScheme
)
```

## Parameters 

`gazetteers`  

The gazetteers to attach to a tag scheme.

`tagScheme`  

The tag scheme for the gazetteers.

## See Also

### Using gazetteers with a tagger

func gazetteers(for: NLTagScheme) -> [NLGazetteer]

Retrieves the gazetteers attached to a tag scheme.

class NLGazetteer

A collection of terms and their labels, which take precedence over a word tagger.

