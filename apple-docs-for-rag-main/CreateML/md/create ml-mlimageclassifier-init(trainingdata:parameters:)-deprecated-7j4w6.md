

- Create ML
- MLImageClassifier
-  init(trainingData:parameters:) Deprecated

Initializer

# init(trainingData:parameters:)

Creates an image classifier with a training dataset represented by a dictionary.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–11.0DeprecatedvisionOS 1.0+

``` source
init(
    trainingData: [String : [URL]],
    parameters: MLImageClassifier.ModelParameters = ModelParameters(validationData: nil)
) throws
```

Deprecated

Use DataSource.filesByLabel to provide dictionary training data instead.

## Parameters 

`trainingData`  

A set of labeled images the task uses to train the image classifier model, contained in a dictionary whose keys are the image labels. Each dictionary value is an array of URLs to images.

`parameters`  

An MLImageClassifier.ModelParameters instance you use to configure the model for the training session.

## Discussion

When you create an MLImageClassifier instance, initialize it with an MLImageClassifier.ModelParameters structure. This allows you to configure the image classifier training process. For example, you can explicitly define the validation dataset instead of allowing the model to choose a random selection of your training data. Alternatively, as shown in the following example, set `validationData` to `nil` to allow the classifier to choose the validation data for you from among your training data. This lets you set other parameters—like maximum iterations and augmentation options—to values other than the default:

```
let parameters = MLImageClassifier.ModelParameters(
    featureExtractor: .scenePrint(revision: 1),
    validationData: nil,
    maxIterations: 20,
    augmentationOptions: [.crop]
)
```

For this particular initialization method—there’s another with the same signature but a different training data type—represent your training data with a dictionary that uses labels as keys. The corresponding values are arrays of URLs that indicate the images associated with that label. In this example, if you have elephant and giraffe images stored in a directory called `Training` within your `Downloads` directory, you can construct a dictionary with the URL of each image:

```
// Get the URL of the directory that holds the validation data.
guard let downloadsURL = FileManager.default.urls(for: .downloadsDirectory, in: .userDomainMask).first
else { fatalError("Can't find Downloads directory") }
let url = downloadsURL.appendingPathComponent("Training")

// For a real classifier, use at least 10 images per label. More is better.
let trainingData = [
    "Elephant": [
        url.appendingPathComponent("Elephant.1.jpg"),
        url.appendingPathComponent("Elephant.2.jpg")
    ],
    "Giraffe": [
        url.appendingPathComponent("Giraffe.1.jpg"),
        url.appendingPathComponent("Giraffe.2.jpg")
    ]
]
```

Note

If you have training data in an MLImageClassifier.DataSource instance, use the similarly named init(trainingData:parameters:) instead. That initialization method takes a data source instead of a dictionary as its training data.

Use the parameter structure and training data to initialize the classifier. Training begins immediately.

```
let classifier = try MLImageClassifier(trainingData: trainingData, parameters: parameters)
```

## See Also

### Training an image classifier synchronously

init(trainingData: MLImageClassifier.DataSource, parameters: MLImageClassifier.ModelParameters) throws

Creates an image classifier with a training dataset represented by a data source.

