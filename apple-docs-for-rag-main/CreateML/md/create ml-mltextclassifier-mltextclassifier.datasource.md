

- Create ML
- MLTextClassifier
-  MLTextClassifier.DataSource 

Enumeration

# MLTextClassifier.DataSource

A data source for a text classifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
enum DataSource
```

## Topics

### Creating a data source

case labeledDirectories(at: URL)

A root directory of labeled directories for your data set.

### Retrieving the data

func labeledTexts() throws -> [String : [String]]

Fetches the labeled data from the data source.

func stratifiedSplit(proportions: [Double], seed: Int, labelColumn: String, textColumn: String) throws -> MLDataTable

Generates a data table by splitting the data source into strata.

## See Also

### Creating and training a text classifier

init(trainingData: [String : [String]], parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: DataFrame, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

init(trainingData: MLTextClassifier.DataSource, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

struct ModelParameters

Parameters that specify model training parameters and validation data.

let modelParameters: MLTextClassifier.ModelParameters

The configuration parameters that the text classifier used for training during initialization.

init(trainingData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLTextClassifier.ModelParameters) throws

Creates a text classifier.

Deprecated

