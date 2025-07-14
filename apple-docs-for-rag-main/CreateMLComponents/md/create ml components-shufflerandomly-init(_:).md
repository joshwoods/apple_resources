

- Create ML Components
- ShuffleRandomly
-  init(\_:) 

Initializer

# init(\_:)

Creates a random shuffle augmentation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(@AugmentationBuilder _ augmentation: () -> RandomTransformer) where Element == RandomTransformer.Input, RandomTransformer : RandomTransformer, RandomTransformer.Input == RandomTransformer.Output
```

## Parameters 

`augmentation`  

An augmentation builder.

