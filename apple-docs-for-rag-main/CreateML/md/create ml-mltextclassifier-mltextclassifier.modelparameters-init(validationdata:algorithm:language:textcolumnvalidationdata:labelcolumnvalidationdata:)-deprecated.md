

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  init(validationData:algorithm:language:textColumnValidationData:labelColumnValidationData:) Deprecated

Initializer

# init(validationData:algorithm:language:textColumnValidationData:labelColumnValidationData:)

Creates parameters for a text classifier with validation data in a data table.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
init(
    validationData: MLDataTable? = nil,
    algorithm: MLTextClassifier.ModelAlgorithmType = .maxEnt(revision: 1),
    language: NLLanguage? = nil,
    textColumnValidationData: String? = nil,
    labelColumnValidationData: String? = nil
)
```

Deprecated

Use the validation property instead.

## Discussion

- validationData: A data table the text classifier uses for validation data during training.

  - algorithm: An algorithm type for the classifier.

  - language: The language of the text to classify.

- textColumnValidationData: The name of the text column in the validation data table.

- labelColumnValidationData: The name of the label column in the validation data table.

## See Also

### Deprecated

init(validationData: [String : [String]], algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a dictionary.

Deprecated

init(validationData: MLTextClassifier.DataSource, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a set of labeled directories.

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

