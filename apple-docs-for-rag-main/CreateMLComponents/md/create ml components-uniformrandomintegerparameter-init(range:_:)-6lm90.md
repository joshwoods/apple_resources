

- Create ML Components
- UniformRandomIntegerParameter
-  init(range:\_:) 

Initializer

# init(range:\_:)

Creates a Random Parameter transformer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    range: Range,
    @AugmentationBuilder _ augmentation: @escaping (Parameter) -> RandomTransformer
) where Input == RandomTransformer.Input
```

## Parameters 

`range`  

The range of a random number to use as input to the transformer.

`augmentation`  

An augmentation builder.

## See Also

### Creating a transformer

init&lt;Input>(range: ClosedRange&lt;Parameter>, (Parameter) -> RandomTransformer)

Creates a Random Parameter transformer.

