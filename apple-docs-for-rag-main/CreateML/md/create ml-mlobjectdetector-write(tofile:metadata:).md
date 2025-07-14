

- Create ML
- MLObjectDetector
-  write(toFile:metadata:) 

Instance Method

# write(toFile:metadata:)

Exports the object detector as a Core ML model file.

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

### Saving an object detector

func write(to: URL, metadata: MLModelMetadata?) throws

Exports the object detector as a Core ML model file.

