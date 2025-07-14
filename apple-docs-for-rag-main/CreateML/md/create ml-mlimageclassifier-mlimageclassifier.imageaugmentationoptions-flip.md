

- Create ML
- MLImageClassifier
- MLImageClassifier.ImageAugmentationOptions
-  flip 

Type Property

# flip

An option for augmenting training data by flipping each image along the horizontal and vertical axes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
static let flip: MLImageClassifier.ImageAugmentationOptions
```

## Discussion

Use this option to tell the image classifier to augment your training data set by flipping the original images.

The classifier creates three new images by flipping the original horizontally, vertically, and both horizontally and vertically.

## See Also

### Selecting augmentation options

static let crop: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by creating cropped versions of each image.

static let rotation: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by rotating each image.

static let blur: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by blurring each image.

static let exposure: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by lightening or darkening each image.

static let noise: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by adding random amounts of noise to each image.

