

- Create ML
- MLObjectDetector
-  write(to:metadata:) 

Instance Method

# write(to:metadata:)

Exports the object detector as a Core ML model file.

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

### Saving an object detector

func write(toFile: String, metadata: MLModelMetadata?) throws

Exports the object detector as a Core ML model file.

