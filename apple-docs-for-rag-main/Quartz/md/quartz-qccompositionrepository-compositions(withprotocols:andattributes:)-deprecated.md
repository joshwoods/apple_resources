

- Quartz
- QCCompositionRepository
-  compositions(withProtocols:andAttributes:) Deprecated

Instance Method

# compositions(withProtocols:andAttributes:)

Returns an array of compositions that match a set of criteria.

macOS 10.4–10.15Deprecated

``` source
func compositions(
    withProtocols protocols: [Any]!,
    andAttributes attributes: [AnyHashable : Any]! = [:]
) -> [Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`protocols`  

The protocols that you want compositions to conform to. Pass `nil` if you don’t want to filter based on the protocol. You can pass any of these protocols: QCCompositionProtocolAnimation, QCCompositionProtocolImageProducer, QCCompositionProtocolImageFilter, QCCompositionProtocolImageCompositor, and QCCompositionProtocolScreenSaverRSS.

`attributes`  

A dictionary that contains the attributes, and their associated values, that you want compositions to match. Pass `nil` if you don’t want to filter based on the attributes. For example, you can pass any of these attributes: QCCompositionAttributeNameKey, QCCompositionAttributeDescriptionKey, QCCompositionAttributeCopyrightKey, and QCCompositionAttributeBuiltInKey.

## Return Value

An array of QCComposition objects that meet the supplied criteria.

## See Also

### Fetching Compositions

func composition(withIdentifier: String!) -> QCComposition!

Returns the composition that corresponds to the identifier.

Deprecated

func allCompositions() -> [Any]!

Returns an array that contains all compositions currently in the composition repository.

Deprecated

