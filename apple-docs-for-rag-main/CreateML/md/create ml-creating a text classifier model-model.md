

- Create ML
-  Creating a text classifier model 

Article

# Creating a text classifier model

Train a machine learning model to classify natural language text.

## Overview

A text classifier is a machine learning model that’s been trained to recognize patterns in natural language text, like the sentiment expressed by a sentence.

You train a text classifier by showing it lots of examples of text you’ve already labeled—for example, movie reviews that you’ve already labeled as positive, negative, or neutral.

### Import your data

Start by gathering textual data and importing it into an MLDataTable instance. You can create a data table from JSON and CSV formats. Or, if your textual data is in a collection of files, you can sort them into folders, using the folder names as labels, similar to the image data source used in Creating an Image Classifier Model.

As an example, consider a JSON file containing movie reviews that you’ve categorized by sentiment. Each entry contains a pair of keys, the `text` and the `label`. The values of those keys are the input samples used to train your model. The JSON snippet below shows three pairs of sentences with their sentiment labels.

```
```

In a macOS playground, create a data frame using the TabularData framework.

```
```

The resulting data frame has two columns, named *text* and *label*, derived from the keys in the JSON file. The column names can be anything, as long as they are meaningful to you, because you’ll use them as parameters in other methods.

### Prepare your data for training and evaluation

The data you use to train your model needs to be different from the data you use to evaluate your model. Use the stratifiedSplit(on:by:randomSeed:) method to split your data into two data frames, one for training and the other for testing. The training data frame contains the majority of your data, and the testing data frame contains the remaining 20 percent.

```
```

### Choose model training parameters

You can use model training parameters to control the learning process. Choose a classifier algorithm type by specifying the MLTextClassifier.ModelAlgorithmType parameter. The MLTextClassifier.ModelAlgorithmType.maxEnt(revision:) algorithm trains quickly and performs well for a wide variety of data. It’s a good starting point algorithm while you’re exploring your data and models.

You can choose a transfer learning algorithm, MLTextClassifier.ModelAlgorithmType.transferLearning(_:revision:). Transfer learning models use a pre-trained model as a feature extractor, you specify the `MLTextClassifier.FeatureExtractorType`. Transfer learning models can take longer to train, but can improve accuracy because the baseline model has already been trained on a large amount of text in a specific language.

If your data contains multiple languages, choose either the maximum entropy algorithm MLTextClassifier.ModelAlgorithmType.maxEnt(revision:) or the transfer learning algorithm MLTextClassifier.ModelAlgorithmType.transferLearning(_:revision:) and set its `MLTextClassifier.FeatureExtractorType` to the Bidirectional Encoder Representations from Transformers (BERT) embedding feature extractor MLTextClassifier.FeatureExtractorType.bertEmbedding.

If your data contains a single language, use the conditional random fields algorithm MLTextClassifier.ModelAlgorithmType.crf(revision:) or the transfer learning algorithm MLTextClassifier.ModelAlgorithmType.transferLearning(_:revision:) and set its `MLTextClassifier.FeatureExtractorType` to the Embeddings from Language Models (ELMo) embedding feature extractor MLTextClassifier.FeatureExtractorType.elmoEmbedding.

Use the MLTextClassifier.ModelParameters.ValidationData parameter to specify the evaluation data that’s held out from training your model. During the training process, use the validation data to estimate your model’s ability to correctly classify new examples. Depending on the validation accuracy, the classifier algorithm might adjust values within the model — or stop the training process, if the accuracy is high enough. Since the split of your data is random, you might get a different result each time you train your model.

```
```

### Create and train a text classifier

Create an instance of MLTextClassifier with your training data frame and the column names.

```
```

To measure how accurately the model (`sentimentClassifier`) performs on the training and validation data, use the classificationError properties of the model’s trainingMetrics and validationMetrics properties.

```
```

### Evaluate a classifier’s accuracy

Next, evaluate your trained model’s performance by testing it against sentences it’s never seen before. Pass your testing data frame to the evaluation(on:) method, which returns an MLClassifierMetrics instance.

```
```

To get the evaluation accuracy, use the classificationError property of the returned MLClassifierMetrics instance.

```
```

If the evaluation performance isn’t good enough, you may need to retrain with more data or make other adjustments. For information about improving model performance, see Improving Your Model’s Accuracy.

### Save a Core ML model

When your model is performing well enough, you’re ready to save it so you can use it in your app. Use the write(to:metadata:) method to write the Core ML model file to disk. Provide any information about the model, like its author, version, or description in an MLModelMetadata instance.

```
```

Specify the file name using the `fileURLWithPath:` parameter, in the above code, `SentimentClassifier.mlmodel`.

### Add a Core ML model to your app

With your app open in Xcode, drag the `SentimentClassifier.mlmodel` file into the navigation pane. Xcode compiles the model and generates a `SentimentClassifier` class for use in your app. Select the `SentimentClassifier.mlmodel` file in Xcode to view additional information about the model.

Create an NLModel in the Natural Language framework from the `SentimentClassifier` to ensure that the tokenization is consistent between training and deployment. Then use predictedLabel(for:) to generate predictions on new text inputs.

```
```

## See Also

### Text Models

Creating a word tagger model

Train a machine learning model to tag individual words in natural language text.

struct MLTextClassifier

A model you train to classify natural language text.

struct MLWordTagger

A word-tagging model you train to classify natural language text at the word level.

struct MLGazetteer

A collection of terms and their labels, which augments a tagger that analyzes natural language text.

struct MLWordEmbedding

A map of strings in a vector space that enable your app to find similar strings by looking at a string’s neighbors.

