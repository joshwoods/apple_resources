

- Natural Language
- NLTagger
-  models(forTagScheme:) 

Instance Method

# models(forTagScheme:)

Returns the models that apply to the given tag scheme.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func models(forTagScheme tagScheme: NLTagScheme) -> [NLModel]
```

## Parameters 

`tagScheme`  

The tag scheme to filter the list of models with.

## Return Value

The array of models that apply to the given tag scheme.

## See Also

### Using models with a tagger

func setModels([NLModel], forTagScheme: NLTagScheme)

Assigns models for a tag scheme.

