

- Create ML
- MLHandPoseClassifier
- MLHandPoseClassifier.ImageAugmentationOptions
-  MLHandPoseClassifier.ImageAugmentationOptions.RawValue 

Type Alias

# MLHandPoseClassifier.ImageAugmentationOptions.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
typealias RawValue = Int
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

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

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

\*\*\*\*Inspect and modify an image augmentation option set with the properties and methods it inherits from standard protocols.

