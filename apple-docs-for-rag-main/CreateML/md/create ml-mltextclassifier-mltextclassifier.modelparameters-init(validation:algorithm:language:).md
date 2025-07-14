

- Create ML
- MLTextClassifier
- MLTextClassifier.ModelParameters
-  init(validation:algorithm:language:) 

Initializer

# init(validation:algorithm:language:)

Creates model parameters for a text classifier with the specified validation data, algorithm, and language.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
init(
    validation: MLTextClassifier.ModelParameters.ValidationData = .split(strategy: .automatic),
    algorithm: MLTextClassifier.ModelAlgorithmType = .maxEnt(revision: 1),
    language: NLLanguage? = nil
)
```

## Parameters 

`validation`  

The validation data to use during text classifier training.

`algorithm`  

An algorithm type for the classifier.

`language`  

The language of the text to classify.

## See Also

### Creating parameters

struct NLLanguage

The languages that the Natural Language framework supports.

enum ModelAlgorithmType

The type of algorithm that a text classifier uses.

enum ValidationData

The validation data that a text classifier uses.

