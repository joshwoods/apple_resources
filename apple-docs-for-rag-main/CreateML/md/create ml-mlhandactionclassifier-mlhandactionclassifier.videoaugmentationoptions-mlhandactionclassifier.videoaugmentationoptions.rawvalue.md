

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  MLHandActionClassifier.VideoAugmentationOptions.RawValue 

Type Alias

# MLHandActionClassifier.VideoAugmentationOptions.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
typealias RawValue = Int
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

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

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

Inspect and modify a video augmentation option set with the properties and methods it inherits from standard protocols.

