

- Quartz
- QCCompositionRepository
-  allCompositions() Deprecated

Instance Method

# allCompositions()

Returns an array that contains all compositions currently in the composition repository.

macOS 10.4–10.15Deprecated

``` source
func allCompositions() -> [Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An array of QCComposition objects.

## See Also

### Fetching Compositions

func composition(withIdentifier: String!) -> QCComposition!

Returns the composition that corresponds to the identifier.

Deprecated

func compositions(withProtocols: [Any]!, andAttributes: [AnyHashable : Any]!) -> [Any]!

Returns an array of compositions that match a set of criteria.

Deprecated

