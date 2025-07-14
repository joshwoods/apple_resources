

- Create ML Components
- ApplyRandomly
-  init(probability:\_:) 

Initializer

# init(probability:\_:)

Creates an apply randomly augmentation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    probability: Double = 0.5,
    @AugmentationBuilder _ augmentation: () -> RandomTransformer
) where Input == RandomTransformer.Input
```

## Parameters 

`probability`  

The probability of applying the transformation. Must be greater than or equal to 0 and less than or equal to 1, the default value is 0.5.

`augmentation`  

The transformer to apply randomly.

