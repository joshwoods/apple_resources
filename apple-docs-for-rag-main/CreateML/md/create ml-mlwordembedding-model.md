

- Create ML
- MLWordEmbedding
-  model 

Instance Property

# model

The word embedding contained within a Core ML model file.

macOS 10.15+

``` source
var model: MLModel { get set }
```

## See Also

### Describing a word embedding

let dimension: Int

The number of dimensions in the vocabulary embedding space.

let vocabularySize: Int

The number of strings in the vocabulary.

var description: String

A text representation of the word embedding.

var debugDescription: String

A text representation of the word embedding that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the word embedding shown in a playground.

