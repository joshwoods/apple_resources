

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  rotate 

Type Property

# rotate

Randomly rotate the pose in a video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static let rotate: MLHandActionClassifier.VideoAugmentationOptions
```

## See Also

### Augmentations supporting types

static let dropFrames: MLHandActionClassifier.VideoAugmentationOptions

Randomly drop frames from a video.

static let horizontallyFlip: MLHandActionClassifier.VideoAugmentationOptions

Apply left-right flips to the pose in a video.

static let interpolateFrames: MLHandActionClassifier.VideoAugmentationOptions

Random time interpolation through a video.

static let scale: MLHandActionClassifier.VideoAugmentationOptions

Randomly scale the pose in a video.

static let translate: MLHandActionClassifier.VideoAugmentationOptions

Randomly translate the pose in a video.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

Option Set Support

Inspect and modify a video augmentation option set with the properties and methods it inherits from standard protocols.

