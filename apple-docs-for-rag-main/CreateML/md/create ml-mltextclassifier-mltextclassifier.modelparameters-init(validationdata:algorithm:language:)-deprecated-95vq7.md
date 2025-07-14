

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  init(validationData:algorithm:language:) Deprecated

Initializer

# init(validationData:algorithm:language:)

Creates parameters for a text classifier with validation data in a set of labeled directories.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
init(
    validationData: MLTextClassifier.DataSource,
    algorithm: MLTextClassifier.ModelAlgorithmType = .maxEnt(revision: 1),
    language: NLLanguage? = nil
)
```

Deprecated

Use the validation property instead.

## Discussion

- validationData: A data source of the labeled directories the text classifier uses for validation data during training.

  - algorithm: An algorithm type for the text classifier.

  - language: The language of the text to classify.

## See Also

### Deprecated

init(validationData: [String : [String]], algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a dictionary.

Deprecated

init(validationData: MLDataTable?, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?, textColumnValidationData: String?, labelColumnValidationData: String?)

Creates parameters for a text classifier with validation data in a data table.

Deprecated

var validationData: MLDataTable?

The validation data.

Deprecated

var textColumnValidationData: String?

The name of the text column in the validation data table.

Deprecated

var labelColumnValidationData: String?

The name of the label column in the validation data table.

Deprecated

