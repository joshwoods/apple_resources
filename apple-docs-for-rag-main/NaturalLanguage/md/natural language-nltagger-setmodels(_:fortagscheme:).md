

- Natural Language
- NLTagger
-  setModels(\_:forTagScheme:) 

Instance Method

# setModels(\_:forTagScheme:)

Assigns models for a tag scheme.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func setModels(
    _ models: [NLModel],
    forTagScheme tagScheme: NLTagScheme
)
```

## Parameters 

`models`  

Array of NLModel objects to be used with this tagger.

`tagScheme`  

The tag scheme the models would be used with.

## Discussion

An array of models is allowed for the case where multiple models need to be used. For example, when models were trained on specific languages.

## See Also

### Using models with a tagger

func models(forTagScheme: NLTagScheme) -> [NLModel]

Returns the models that apply to the given tag scheme.

