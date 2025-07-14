

- Create ML Components
-  RandomImageCropper 

Structure

# RandomImageCropper

Crops an image at a random location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct RandomImageCropper
```

## Topics

### Creating an image cropper

init(scale: ClosedRange&lt;Double>, aspectRatio: Double?)

Creates an augmentation that crops an input image at a random location with a scale that indicates the lower and upper bounds to randomly scale the height and width of the image. The range must be between 0 and 1.

init(targetSize: CGSize)

Creates an augmentation that crops an input image at a random location to the specified target size.

init(targetWidth: Double, targetHeight: Double)

Creates an augmentation that crops an input image at a random location to the specified target width and height.

### Performing the augmentation

func applied(to: CIImage, generator: inout some RandomNumberGenerator, eventHandler: EventHandler?) async throws -> CIImage

Randomly crops an image at a random location of a given size.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

## Relationships

### Conforms To

- RandomTransformer
- Sendable

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

struct ShuffleRandomly

Apply transformations in a random order.

struct UniformRandomFloatingPointParameter

Applies the transformer with a randomly generated input parameter.

class UniformRandomIntegerParameter

Applies the transformer with a randomly generated input parameter.

struct UpsampledAugmentationSequence

An async sequence of augmented elements.

