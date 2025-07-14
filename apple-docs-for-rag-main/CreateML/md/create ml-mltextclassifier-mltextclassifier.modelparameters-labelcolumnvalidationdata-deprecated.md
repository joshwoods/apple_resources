

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  labelColumnValidationData Deprecated

Instance Property

# labelColumnValidationData

The name of the label column in the validation data table.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
var labelColumnValidationData: String? { get set }
```

Deprecated

Use the validation property instead.

## See Also

### Deprecated

init(validationData: [String : [String]], algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?)

Creates parameters for a text classifier with validation data in a dictionary.

Deprecated

init(validationData: MLDataTable?, algorithm: MLTextClassifier.ModelAlgorithmType, language: NLLanguage?, textColumnValidationData: String?, labelColumnValidationData: String?)

Creates parameters for a text classifier with validation data in a data table.

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

