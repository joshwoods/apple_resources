

- Create ML
- MLImageClassifier
- MLImageClassifier.ImageAugmentationOptions
-  blur 

Type Property

# blur

An option for augmenting training data by blurring each image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
static let blur: MLImageClassifier.ImageAugmentationOptions
```

## Discussion

Use this option to tell the image classifier to augment your training data set by creating blurred versions of the original images.

The classifier creates four new images with random amounts of blur for each original.

## See Also

### Selecting augmentation options

static let crop: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by creating cropped versions of each image.

static let rotation: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by rotating each image.

static let exposure: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by lightening or darkening each image.

static let noise: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by adding random amounts of noise to each image.

static let flip: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by flipping each image along the horizontal and vertical axes.

