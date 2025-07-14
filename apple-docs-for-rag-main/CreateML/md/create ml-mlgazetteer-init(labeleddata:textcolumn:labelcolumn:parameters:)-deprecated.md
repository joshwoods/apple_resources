

- Create ML
- MLGazetteer
-  init(labeledData:textColumn:labelColumn:parameters:) Deprecated

Initializer

# init(labeledData:textColumn:labelColumn:parameters:)

Creates a gazetteer from a table of labels and terms.

macOS 10.15–14.0Deprecated

``` source
init(
    labeledData: MLDataTable,
    textColumn: String,
    labelColumn: String,
    parameters: MLGazetteer.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`labeledData`  

A table of labels and terms.

`textColumn`  

The name of the column containing the terms.

`labelColumn`  

The name of the column containing the labels.

`parameters`  

The model parameters.

## See Also

### Creating a gazetteer

init(dictionary: [String : [String]], parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a dictionary of labels and terms.

struct ModelParameters

The model configuration parameters.

let modelParameters: MLGazetteer.ModelParameters

The model configuration parameters.

