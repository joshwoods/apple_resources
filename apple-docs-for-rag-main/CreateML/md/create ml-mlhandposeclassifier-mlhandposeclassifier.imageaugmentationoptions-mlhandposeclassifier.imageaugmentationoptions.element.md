

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ImageAugmentationOptions
-  MLHandPoseClassifier.ImageAugmentationOptions.Element 

Type Alias

# MLHandPoseClassifier.ImageAugmentationOptions.Element

The element type of the option set.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
typealias Element = MLHandPoseClassifier.ImageAugmentationOptions
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

## See Also

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

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

\*\*\*\*Inspect and modify an image augmentation option set with the properties and methods it inherits from standard protocols.

