

- Create ML
- MLGazetteer
-  MLGazetteer.ModelParameters 

Structure

# MLGazetteer.ModelParameters

The model configuration parameters.

macOS 10.15+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(language: NLLanguage?)

Creates model parameters.

### Accessing parameters

var language: NLLanguage?

The language setting.

### Describing parameters

var description: String

A text representation of the gazetteer settings.

var debugDescription: String

A text representation of the gazetteer settings that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the gazetteer settings shown in a playground.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Sendable

## See Also

### Creating a gazetteer

init(dictionary: [String : [String]], parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a dictionary of labels and terms.

init(labeledData: MLDataTable, textColumn: String, labelColumn: String, parameters: MLGazetteer.ModelParameters) throws

Creates a gazetteer from a table of labels and terms.

Deprecated

let modelParameters: MLGazetteer.ModelParameters

The model configuration parameters.

