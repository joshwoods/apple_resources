

- Create ML
- MLWordEmbedding
-  MLWordEmbedding.ModelParameters 

Structure

# MLWordEmbedding.ModelParameters

The model configuration parameters.

macOS 10.15+

``` source
struct ModelParameters
```

## Topics

### Creating parameters

init(language: NLLanguage?, revision: Int)

Creates model parameters.

### Accessing parameters

var revision: Int

The revision of the word embedding.

var language: NLLanguage?

The language of the word embedding.

### Describing parameters

var description: String

A text representation of the word embedding parameters.

var debugDescription: String

A text representation of the word embedding parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the word embedding parameters shown in a playground.

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

### Creating a word embedding

init(dictionary: [String : [Double]], parameters: MLWordEmbedding.ModelParameters) throws

Creates a word embedding.

let modelParameters: MLWordEmbedding.ModelParameters

The model configuration parameters.

