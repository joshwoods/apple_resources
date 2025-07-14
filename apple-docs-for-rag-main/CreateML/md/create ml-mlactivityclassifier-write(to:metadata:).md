

- Create ML
- MLActivityClassifier
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the activity classifier as a Core ML model file.

macOS 10.15+

``` source
func write(
    to fileURL: URL,
    metadata: MLModelMetadata? = MLModelMetadata()
) throws
```

## Parameters 

`fileURL`  

A file-system URL.

`metadata`  

The model’s description, author, version, and license information.

## See Also

### Saving an activity classifier

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the activity classifier as a Core ML model file.

