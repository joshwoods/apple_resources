

- Create ML
- MLGazetteer
-  modelParameters 

Instance Property

# modelParameters

The model configuration parameters.

macOS 10.15+

``` source
let modelParameters: MLGazetteer.ModelParameters
```

## See Also

### Creating a gazetteer

init(dictionary: [String : [String]], parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a dictionary of labels and terms.

init(labeledData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a table of labels and terms.

Deprecated

struct ModelParameters

The model configuration parameters.

