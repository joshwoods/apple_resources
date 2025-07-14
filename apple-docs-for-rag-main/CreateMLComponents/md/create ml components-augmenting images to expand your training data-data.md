

- Create ML Components
-  Augmenting images to expand your training data 

Article

# Augmenting images to expand your training data

Improve your model by using transformed versions of your training images.

## Overview

Training a good image model requires a variety of training images with different characteristics. If you’re training an image classifier to recognize flowers you can improve classification accuracy by providing flower photos with a variety of lighting conditions, angles, and backgrounds. However, collecting and labeling images is a time-consuming process.

To maximize the potential impact of your data you can use image augmentations. Augmenting images is the process of applying transformations such as flipping, cropping, resizing, adjusting brightness, adding noise, and so on. Image augmentations are not a replacement for a good image data set, but they help maximize the data set’s effectiveness. Each augmentation has the potential to multiply the size of your training data which is helpful when your training sample size is small.

Keep in mind that performing augmentations has some drawbacks. You can’t reuse extracted features across training iterations because each iteration produces a new set of augmented images. This increase in training time can be significant. Augmentations have the most impact when your dataset is small relative to the number of parameters in your model.

### Write an augmentation

You can use Augmenter to create a custom augmentation. The augmenter applies each transformer to each image in sequence. For example, this augmenter randomly flips (with 50% probability) and then randomly crops images:

```
```

To generate a random number each time, use UniformRandomFloatingPointParameter. You can use the random number with any transformer. For instance, to perform a slight rotation using ImageRotator:

```
```

### Apply augmentations to your training data

After you create an augmenter, you can use it to augment your training data. You do this with the applied(to:) method:

```
```

Because augmentations are usually random, it makes sense to do more than one pass over your training data. Each pass results in a different set of images, for instance with different scale factors. You can control the number of passes by using the applied(to:upsampledBy:) method. For instance, to get 10 times the number of images:

```
```

Note

The result of the augmentations is an asynchronous sequence. The augmenter doesn’t perform augmentations until you request them to avoid the memory overhead.

### Train an image classifier

You can now use your augmented data set to train an image classifier. Because augmentations take images, not URLs, you may need to read your files first.

```
```

Now that you have annotated images, the next step is to create your pipeline. For an image classifier, create a feature extractor and a classifier.

```
```

Next, create the augmenter that transforms the training images.

```
```

Finally, create a model, apply the augmenter to the training data, and progressively train the model using update(_:with:eventHandler:). The following example applies the `augmenter` to the `trainingImages` and updates the `model` up to 100 times:

```
```

The example above applies the `augmenter` to shuffled images. Shuffling images creates more variation, which helps prevent over-fitting. The example breaks the data into batches after each augmentation, and updates the model with each `batch`. Using a smaller batch size typically produces a better model, while using a larger batch size can speed up training.

Tip

A batch size of 32 is often a good starting point.

### Stop training

Training your model progressively using the update(_:with:eventHandler:) method lets you control when to stop training. Stop training when the validation accuracy stops improving, for example:

```
```

## See Also

### Related Documentation

struct Augmenter

An augmenter.

struct ApplyEachRandomly

Applies each transformer randomly given a probability.

struct ApplyRandomly

Randomly applies the transformer with the given probability.

struct ChooseRandomly

Apply single transformation randomly chosen from a list of transformers.

struct RandomImageCropper

Crops an image at a random location.

protocol RandomTransformer

A transformer that takes an input and a random number generator and produces a randomized output.

struct ShuffleRandomly

Apply transformations in a random order.

struct UniformRandomFloatingPointParameter

Applies the transformer with a randomly generated input parameter.

class UniformRandomIntegerParameter

Applies the transformer with a randomly generated input parameter.

### Image components

Creating a multi-label image classifier

Train a machine learning model to assign multiple labels to an image.

struct ImageReader

An image file reader.

protocol ImageFeatureExtractor

A transformer that takes an image and outputs image features.

struct ImageCropper

An image crop transformer.

struct ImageScaler

An image scaling transformer.

struct ImageFeaturePrint

ImageFeaturePrint image feature extractor.

struct ImageBlur

An image blurring transformer.

struct ImageColorTransformer

An image color transformer.

struct ImageExposureAdjuster

An image exposure adjusting transformer.

struct ImageFlipper

An image flipper transformer.

struct ImageRotator

An image rotating transformer.

struct RandomImageNoiseGenerator

A transformer that adds random noise to an image.

struct MLModelImageFeatureExtractor

An image feature extractor provided by an MLModel.

