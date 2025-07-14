

- Create ML
- MLWordEmbedding
-  init(dictionary:parameters:) 

Initializer

# init(dictionary:parameters:)

Creates a word embedding.

macOS 10.15+

``` source
init(
    dictionary: [String : [Double]],
    parameters: MLWordEmbedding.ModelParameters = ModelParameters()
) throws
```

## Parameters 

`dictionary`  

A dictionary of strings and their embeddings.

`parameters`  

The model parameters.

## See Also

### Creating a word embedding

struct ModelParameters

The model configuration parameters.

let modelParameters: MLWordEmbedding.ModelParameters

The model configuration parameters.

