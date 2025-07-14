

- Create ML Components
-  UniformRandomIntegerParameter 

Class

# UniformRandomIntegerParameter

Applies the transformer with a randomly generated input parameter.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
final class UniformRandomIntegerParameter where RandomTransformer : RandomTransformer, Parameter : FixedWidthInteger, RandomTransformer.Input == RandomTransformer.Output
```

## Overview

The parameter is chosen from a discrete uniform distribution in the specified range.

Note that a new transformer is created every time this transformer is applied. This may cause performance issues if the embedded transformer creation is costly.

## Topics

### Creating a transformer

init&lt;Input>(range: ClosedRange&lt;Parameter>, (Parameter) -> RandomTransformer)

Creates a Random Parameter transformer.

init&lt;Input>(range: Range&lt;Parameter>, (Parameter) -> RandomTransformer)

Creates a Random Parameter transformer.

### Getting the range

var range: Range&lt;Parameter>

The range of a random number to use as input to the transformer.

### Applying

func applied(to: RandomTransformer.Input, generator: inout some RandomNumberGenerator, eventHandler: EventHandler?) async throws -> RandomTransformer.Output

Performs the random apply operation on the input.

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

struct ChooseRandomly

Apply single transformation randomly chosen from a list of transformers.

struct RandomImageCropper

Crops an image at a random location.

struct ShuffleRandomly

Apply transformations in a random order.

struct UniformRandomFloatingPointParameter

Applies the transformer with a randomly generated input parameter.

struct UpsampledAugmentationSequence

An async sequence of augmented elements.

