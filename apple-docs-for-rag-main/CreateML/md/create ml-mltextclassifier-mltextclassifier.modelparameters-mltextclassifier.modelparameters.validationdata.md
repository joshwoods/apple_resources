

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  MLTextClassifier.ModelParameters.ValidationData 

Enumeration

# MLTextClassifier.ModelParameters.ValidationData

The validation data that a text classifier uses.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
enum ValidationData
```

## Mentioned in 

Creating a text classifier model

## Topics

### Specifying validation data

case split(strategy: MLSplitStrategy)

Generates the validation data by splitting the training dataset.

case table(MLDataTable, textColumn: String, labelColumn: String)

Sets the validation data from the provided data table.

case dataFrame(DataFrame, textColumn: String, labelColumn: String)

Set validation data from the MLDataTable provided.

case dataSource(MLTextClassifier.DataSource)

Sets the validation data from the provided data source.

case dictionary([String : [String]])

Sets the validation data from the provided dictionary.

case none

Doesn’t set validation data.

## See Also

### Creating parameters

init(validation: MLTextClassifier.ModelParameters.ValidationData, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates model parameters for a text classifier with the specified validation data, algorithm, and language.

struct NLLanguage

The languages that the Natural Language framework supports.

enum ModelAlgorithmType

The type of algorithm that a text classifier uses.

