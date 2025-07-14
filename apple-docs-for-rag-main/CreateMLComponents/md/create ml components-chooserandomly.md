

- Create ML Components
-  ChooseRandomly 

Structure

# ChooseRandomly

Apply single transformation randomly chosen from a list of transformers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
struct ChooseRandomly
```

## Topics

### Creating an augmentation

init&lt;RandomTransformer>(() -> RandomTransformer)

Creates a choose randomly augmentation.

### Applying transformers

func applied(to: Element, generator: inout some RandomNumberGenerator, eventHandler: EventHandler?) async throws -> Element

Chooses a random transformer from a list of transformers and applies the chosen transformer.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

## Relationships

### Conforms To

- RandomTransformer

## See Also

### Augmentations

struct ApplyEachRandomly

Applies each transformer randomly given a probability.

struct ApplyRandomly

Randomly applies the transformer with the given probability.

struct AugmentationBuilder

A series of augmentations.

struct AugmentationSequence

An async sequence of augmented elements.

struct Augmenter

An augmenter.

struct RandomImageCropper

Crops an image at a random location.

struct ShuffleRandomly

Apply transformations in a random order.

struct UniformRandomFloatingPointParameter

Applies the transformer with a randomly generated input parameter.

class UniformRandomIntegerParameter

Applies the transformer with a randomly generated input parameter.

struct UpsampledAugmentationSequence

An async sequence of augmented elements.

