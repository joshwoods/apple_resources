

- Create ML
-  Creating a Text Classifier Model 

Article

# Creating a Text Classifier Model

Train a machine learning model to classify natural language text.

## Overview

A text classifier is a machine learning model that’s been trained to recognize patterns in natural language text, like the sentiment expressed by a sentence.

You train a text classifier by showing it lots of examples of text you’ve already labeled—for example, movie reviews that you’ve already labeled as positive, negative, or neutral.

### Import Your Data

Start by gathering textual data and importing it into an MLDataTable instance. You can create a data table from JSON and CSV formats. Or, if your textual data is in a collection of files, you can sort them into folders, using the folder names as labels, similar to the image data source used in Creating an Image Classifier Model.

As an example, consider a JSON file containing movie reviews that you’ve categorized by sentiment. Each entry contains a pair of keys, the `text` and the `label`. The values of those keys are the input samples used to train your model. The JSON snippet below shows three pairs of sentences with their sentiment labels.

```
// JSON file
[
    {
        "text": "The movie was fantastic!",
        "label": "positive"
    }, {
        "text": "Very boring. Fell asleep.",
        "label": "negative"
    }, {
        "text": "It was just OK.",
        "label": "neutral"
    } ...
]
```

In a macOS playground, create the data table using the init(contentsOf:options:) method of MLDataTable.

```
import CreateML

let data = try MLDataTable(contentsOf: URL(fileURLWithPath: ""))
```

The resulting data table has two columns, named *text* and *label*, derived from the keys in the JSON file. The column names can be anything, as long as they are meaningful to you, because you’ll use them as parameters in other methods.

### Prepare Your Data for Training and Evaluation

The data you use to train the model needs to be different from the data you use to evaluate the model. Use the randomSplit(by:seed:) method of MLDataTable to split your data into two tables, one for training and the other for testing. The training data table contains the majority of your data, and the testing data contains the remaining 10 to 20 percent.

```
let (trainingData, testingData) = data.randomSplit(by: 0.8, seed: 5)
```

### Create and Train the Text Classifier

Create an instance of MLTextClassifier with your training data table and the names of your columns. Training begins right away.

```
let sentimentClassifier = try MLTextClassifier(trainingData: trainingData,
                                               textColumn: "text",
                                               labelColumn: "label")
```

During training, Create ML puts aside a small percentage of the training data to use for validating the model’s progress during the training phase. The validation data allows the training process to gauge the model’s performance on examples the model hasn’t been trained on. Depending on the validation accuracy, the training algorithm could adjust values within the model or even stop the training process, if the accuracy is high enough. Because the split is done randomly, you might get a different result each time you train the model.

To see how accurately the model performed on the training and validation data, use the classificationError properties of the model’s trainingMetrics and validationMetrics properties.

```
// Training accuracy as a percentage
let trainingAccuracy = (1.0 - sentimentClassifier.trainingMetrics.classificationError) * 100

// Validation accuracy as a percentage
let validationAccuracy = (1.0 - sentimentClassifier.validationMetrics.classificationError) * 100
```

### Evaluate the Classifier’s Accuracy

Next, evaluate your trained model’s performance by testing it against sentences it’s never seen before. Pass your testing data table to the evaluation(on:) method, which returns an MLClassifierMetrics instance.

```
let evaluationMetrics = sentimentClassifier.evaluation(on: testingData)
```

To get the evaluation accuracy, use the classificationError property of the returned MLClassifierMetrics instance.

```
// Evaluation accuracy as a percentage
let evaluationAccuracy = (1.0 - evaluationMetrics.classificationError) * 100
```

If the evaluation performance isn’t good enough, you may need to retrain with more data or make other adjustments. For information about improving model performance, see Improving Your Model’s Accuracy.

### Save the Core ML Model

When your model is performing well enough, you’re ready to save it so you can use it in your app. Use the write(to:metadata:) method to write the Core ML model file (`SentimentClassifier.mlmodel`) to disk. Provide any information about the model, like its author, version, or description in an MLModelMetadata instance.

```
let metadata = MLModelMetadata(author: "John Appleseed",
                               shortDescription: "A model trained to classify movie review sentiment",
                               version: "1.0")

try sentimentClassifier.write(to: URL(fileURLWithPath: ""),
                              metadata: metadata)
```

### Add the Model to Your App

With your app open in Xcode, drag the `SentimentClassifier.mlmodel` file into the navigation pane. Xcode compiles the model and generates a `SentimentClassifier` class for use in your app. Select the `SentimentClassifier.mlmodel` file in Xcode to view additional information about the model.

Create an NLModel in the Natural Language framework from the `SentimentClassifier` to ensure that the tokenization is consistent between training and deployment. Then use predictedLabel(for:) to generate predictions on new text inputs.

```
import NaturalLanguage
import CoreML

let mlModel = try SentimentClassifier(configuration: MLModelConfiguration()).model

let sentimentPredictor = try NLModel(mlModel: mlModel)
sentimentPredictor.predictedLabel(for: "It was the best I've ever seen!")
```

