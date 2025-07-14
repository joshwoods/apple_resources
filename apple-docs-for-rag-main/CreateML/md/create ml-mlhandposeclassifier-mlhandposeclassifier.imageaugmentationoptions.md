

- Create ML
- MLHandPoseClassifier
-  MLHandPoseClassifier.ImageAugmentationOptions 

Structure

# MLHandPoseClassifier.ImageAugmentationOptions

Options a hand pose classification training session can use to generate additional training data from the images you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct ImageAugmentationOptions
```

## Topics

### Augmentations supporting types

static let horizontallyFlip: MLHandPoseClassifier.ImageAugmentationOptions

Apply left-right flips to the pose in an image.

static let rotate: MLHandPoseClassifier.ImageAugmentationOptions

Randomly rotate the pose in an image.

static let scale: MLHandPoseClassifier.ImageAugmentationOptions

Randomly scale the pose in an image.

static let translate: MLHandPoseClassifier.ImageAugmentationOptions

Randomly translate the pose in an image.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

\*\*\*\*Inspect and modify an image augmentation option set with the properties and methods it inherits from standard protocols.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Parameter supporting types

enum ValidationData

A dataset a hand pose classifier task uses to validate the model during a training session.

enum ModelAlgorithmType

The hand pose classifier training algorithm options.

