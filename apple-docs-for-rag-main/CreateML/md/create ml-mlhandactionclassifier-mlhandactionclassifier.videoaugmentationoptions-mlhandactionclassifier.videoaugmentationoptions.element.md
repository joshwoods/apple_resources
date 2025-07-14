

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  MLHandActionClassifier.VideoAugmentationOptions.Element 

Type Alias

# MLHandActionClassifier.VideoAugmentationOptions.Element

The element type of the option set.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
typealias Element = MLHandActionClassifier.VideoAugmentationOptions
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

## See Also

### Augmentations supporting types

static let dropFrames: MLHandActionClassifier.VideoAugmentationOptions

Randomly drop frames from a video.

static let horizontallyFlip: MLHandActionClassifier.VideoAugmentationOptions

Apply left-right flips to the pose in a video.

static let interpolateFrames: MLHandActionClassifier.VideoAugmentationOptions

Random time interpolation through a video.

static let rotate: MLHandActionClassifier.VideoAugmentationOptions

Randomly rotate the pose in a video.

static let scale: MLHandActionClassifier.VideoAugmentationOptions

Randomly scale the pose in a video.

static let translate: MLHandActionClassifier.VideoAugmentationOptions

Randomly translate the pose in a video.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

Inspect and modify a video augmentation option set with the properties and methods it inherits from standard protocols.

