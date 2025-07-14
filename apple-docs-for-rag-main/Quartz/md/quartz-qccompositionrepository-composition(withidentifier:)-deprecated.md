

- Quartz
- QCCompositionRepository
-  composition(withIdentifier:) Deprecated

Instance Method

# composition(withIdentifier:)

Returns the composition that corresponds to the identifier.

macOS 10.4–10.15Deprecated

``` source
func composition(withIdentifier identifier: String!) -> QCComposition!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`identifier`  

A string that uniquely identifies the composition to retrieve.

## Return Value

The composition identified by the provided string, or `nil` if there is no composition with that identifier in the composition repository.

## See Also

### Fetching Compositions

func compositions(withProtocols: [Any]!, andAttributes: [AnyHashable : Any]!) -> [Any]!

Returns an array of compositions that match a set of criteria.

Deprecated

func allCompositions() -> [Any]!

Returns an array that contains all compositions currently in the composition repository.

Deprecated

