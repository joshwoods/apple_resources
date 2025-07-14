

- Create ML
- MLActivityClassifier
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the activity classifier as a Core ML model file.

macOS 10.15+

``` source
func write(
    toFile path: String,
    metadata: MLModelMetadata? = MLModelMetadata()
) throws
```

## Parameters 

`path`  

A file-system path.

`metadata`  

The model’s description, author, version, and license information.

## See Also

### Saving an activity classifier

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the activity classifier as a Core ML model file.

