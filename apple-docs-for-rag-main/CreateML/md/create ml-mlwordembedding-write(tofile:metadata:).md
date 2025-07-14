

- Create ML
- MLWordEmbedding
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the word embedding as a Core ML model file at the specified file path.

macOS 10.15+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`path`  

A file system path where the model file should be written.

`metadata`  

Descriptive information to include with the exported model file.

## See Also

### Saving a word embedding

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the word embedding as a Core ML model file at the specified URL.

