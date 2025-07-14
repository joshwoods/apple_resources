

- Create ML
- MLRecommender
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the recommender as a Core ML model file at the given URL.

macOS 10.15+

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

### Saving a recommender

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the recommender as a Core ML model file at the given file path.

