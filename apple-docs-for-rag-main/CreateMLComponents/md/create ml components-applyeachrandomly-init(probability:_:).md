

- Create ML Components
- ApplyEachRandomly
-  init(probability:\_:) 

Initializer

# init(probability:\_:)

Creates an augmentation that applies each transformer randomly in the given order.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    probability: Double = 0.5,
    @AugmentationBuilder _ augmentation: () -> RandomTransformer
) where Element == RandomTransformer.Input, RandomTransformer : RandomTransformer, RandomTransformer.Input == RandomTransformer.Output
```

## Parameters 

`probability`  

The probability of applying each transformer. Default value is 0.5.

`augmentation`  

An augmentation builder.

