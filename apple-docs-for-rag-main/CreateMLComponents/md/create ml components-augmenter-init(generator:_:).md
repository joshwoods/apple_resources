

- Create ML Components
- Augmenter
-  init(generator:\_:) 

Initializer

# init(generator:\_:)

Creates an augmenter from a random number generator and an augmentation builder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    generator: RandomNumberGenerator = SystemRandomNumberGenerator(),
    @AugmentationBuilder _ builder: @escaping () -> RandomTransformer
) where Input == RandomTransformer.Input
```

## Parameters 

`generator`  

A random number generator.

`builder`  

An augmentation builder.

