

- Create ML
- MLGazetteer
-  init(dictionary:parameters:) 

Initializer

# init(dictionary:parameters:)

Creates a gazetteer from a dictionary of labels and terms.

macOS 10.15+

``` source
init(
    dictionary: [String : [String]],
    parameters: MLGazetteer.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`dictionary`  

A dictionary of labels and terms.

`parameters`  

The model parameters.

## See Also

### Creating a gazetteer

init(labeledData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a table of labels and terms.

Deprecated

struct ModelParameters

The model configuration parameters.

let modelParameters: MLGazetteer.ModelParameters

The model configuration parameters.

