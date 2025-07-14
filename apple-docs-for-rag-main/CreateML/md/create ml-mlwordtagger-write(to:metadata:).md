

- Create ML
- MLWordTagger
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the word tagger as a Core ML model file at the specified URL.

macOS 10.14+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = nil
) throws
```

## Parameters 

`fileURL`  

The location in the file system to which the file should be written.

`metadata`  

Descriptive information to include with the exported model file.

## See Also

### Saving a word tagger

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the word tagger as a Core ML model file at the specified file path.

